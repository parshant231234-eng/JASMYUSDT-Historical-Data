# JASMYUSDT 1-Minute Historical Kline Dataset

An institutional-grade, open-source archive of cleaned, standardized, and validated **1-minute intraday historical kline data** for **JASMYUSDT** (Binance Spot).

---

## 📊 Dataset Specifications
- **Symbol:** `JASMYUSDT`
- **Market:** Binance Spot
- **Timeframe:** 1 Minute (`1m`)
- **Total Months:** `60` months
- **Total Candles:** `2,575,360` 1-minute candles
- **Historical Range:** `2021-11-22 12:00:00` to `2026-10-15 23:59:00` (UTC)
- **Schema:** `timestamp, datetime_utc, open, high, low, close, volume, quote_volume, trade_count, taker_buy_volume, taker_buy_quote_volume`

---

## 🏛️ Directory Hierarchy
```text
JASMYUSDT-Historical-Data/
├── README.md
└── 1m/
    └── <YYYY>/
        └── <MM>/
            └── JASMYUSDT_1m_<YYYY-MM>.csv
```

---

## ⚡ 1-Line Pandas Stream Loader
Load any month directly from GitHub's raw CDN without cloning the repository:

```python
import pandas as pd

url = "https://raw.githubusercontent.com/parshant231234-eng/JASMYUSDT-Historical-Data/main/1m/2026/10/JASMYUSDT_1m_2026-10.csv"
df = pd.read_csv(url)
print(df.head())
```
