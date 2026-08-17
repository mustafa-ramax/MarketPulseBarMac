# MarketPulseBar

**A native macOS menu bar stock ticker and market tracker for stocks, crypto, ETFs, forex, indices, commodities, and portfolio P/L.**

MarketPulseBar keeps the market visible while you work, without making you keep a trading dashboard, chart window, or browser tab open all day.

[**Explore MarketPulseBar →**](https://mustafaramx.com/apps/marketpulsebar/) ·
[Watch the demo](https://www.youtube.com/watch?v=_PoSTb12ScQ) ·
[Read the build story](https://mustafaramx.com/post/marketpulsebar-track-crypto-stocks-etfs-gold-silver-p-l-in-your-mac-menu-bar/) ·
[Report a bug](../../issues/new?template=bug_report.md) ·
[Request a feature](../../issues/new?template=feature_request.md)

> **Closed-source app**
>
> This is the official public product, documentation, and support repository for MarketPulseBar.  
> The application source code is proprietary and is **not distributed in this repository**.

---

## Why MarketPulseBar?

Most stock trackers and portfolio apps are designed around dashboards: charts, news, watchlists, indicators, research tools, and multiple panels competing for attention.

MarketPulseBar takes a smaller approach.

It puts the prices and positions you care about directly in the **Mac menu bar**, so you can glance at stocks, crypto, ETFs, forex, indices, gold, silver, and other supported commodities without interrupting your work.

The goal is simple:

> **Market awareness should take one glance, not a browser tab.**

---

## Features

- **macOS menu bar market tracking** for stocks, crypto, ETFs, forex, indices, gold, silver, and other supported commodities
- **Configurable watchlists** for the symbols that matter to you
- **Price-only mode** for a clean view of current prices and movement
- **Portfolio mode** with units and average cost for at-a-glance profit/loss tracking
- **Price alerts** so you do not need to stare at the market
- **Multi mode** to keep several symbols visible at once
- **Rotate mode** to cycle through a larger watchlist
- **Hybrid mode** to keep important symbols fixed while others rotate
- **Compact mode** for smaller displays and reduced menu bar clutter
- **Quick-glance sparklines** for a lightweight visual signal of recent movement
- **Yahoo Finance market coverage** for supported symbols and instruments
- **Native Swift and SwiftUI interface** designed specifically for the macOS menu bar
- Adaptive polling, backoff, and cached values to keep the experience responsive and lightweight

---

## Track multiple markets from your Mac menu bar

MarketPulseBar uses Yahoo Finance as its market-data source and follows the instruments and symbols available through Yahoo Finance.

| Market | Examples of what you can track |
|---|---|
| Stocks | Individual equities supported by Yahoo Finance |
| Crypto | Cryptocurrency market symbols |
| ETFs | Exchange-traded funds |
| Forex | Currency pairs |
| Indices | Market indices |
| Commodities | Gold, silver, and other supported commodities |

Market coverage and symbol behaviour depend on Yahoo Finance availability.

---

## Price-only mode

Sometimes you do not need a portfolio dashboard. You just want to know what a market is doing.

Price-only mode keeps MarketPulseBar focused on:

- the symbol
- its current price
- market movement

That makes it useful as a lightweight **Mac stock ticker**, **crypto price tracker**, or general **menu bar market watcher** while you are coding, researching, writing, or working.

---

## Portfolio P/L tracking

MarketPulseBar can also act as a compact **portfolio P/L tracker**.

Add:

- your units
- your average cost

MarketPulseBar can then show your current profit or loss directly from the menu bar, helping you answer a simple question quickly:

**How is my tracked position doing right now?**

It is intentionally not a brokerage platform or full portfolio-management terminal. MarketPulseBar is designed for quick awareness, not order execution or deep investment research.

---

## Menu bar display modes

A Mac menu bar has very limited space, especially when you want to monitor more than one ticker.

MarketPulseBar provides several display modes so you can choose how much information remains visible.

| Mode | Best for |
|---|---|
| **Multi** | Showing several market symbols side by side |
| **Rotate** | Cycling through a larger watchlist |
| **Hybrid** | Keeping priority symbols fixed while the rest rotate |
| **Compact** | Saving menu bar space and reducing visual clutter |

This lets MarketPulseBar work as both a focused **macOS stock ticker** and a broader multi-asset market tracker.

---

## Screenshots

> Add the four MarketPulseBar screenshots to the `assets/` directory before publishing this repository.  
> Recommended filenames are documented in [`assets/README.md`](assets/README.md).

### Watchlist

![MarketPulseBar watchlist with stocks, crypto, ETFs, forex, gold and silver](assets/marketpulsebar-watchlist.png)

### Mac menu bar ticker

![MarketPulseBar stock and crypto ticker in the macOS menu bar](assets/marketpulsebar-menu-bar-ticker.png)

### Display controls

![MarketPulseBar menu bar display controls](assets/marketpulsebar-display-controls.png)

### Settings

![MarketPulseBar watchlist, refresh and display settings](assets/marketpulsebar-settings.png)

---

## Video demo

See MarketPulseBar running on macOS:

[![Watch the MarketPulseBar macOS menu bar demo](https://img.youtube.com/vi/_PoSTb12ScQ/maxresdefault.jpg)](https://www.youtube.com/watch?v=_PoSTb12ScQ)

**[Watch the full MarketPulseBar demo on YouTube →](https://www.youtube.com/watch?v=_PoSTb12ScQ)**

---

## Native macOS app

MarketPulseBar was designed and shipped independently in **Swift** and **SwiftUI**.

It uses `MenuBarExtra` so the app behaves like a focused macOS menu bar utility instead of a traditional finance dashboard.

Its sparklines are drawn with SwiftUI Canvas, while the data layer adapts its polling cadence, backs off when appropriate, and caches the last available values so the interface can remain useful when a market-data request is delayed.

The app is built around the constraints of the Mac menu bar rather than treating the menu bar as an afterthought.

---

## Who is MarketPulseBar for?

MarketPulseBar is designed for people who want quick market awareness while they work, including:

- investors
- traders
- developers
- researchers
- crypto market watchers
- ETF investors
- anyone who repeatedly checks a small group of market symbols during the day

If you need technical analysis, order execution, extensive historical research, or a complete brokerage experience, a dedicated trading or research platform will be a better fit.

If you mainly want to know **what your markets are doing without opening another dashboard**, MarketPulseBar is built for that job.

---

## FAQ

### Is MarketPulseBar a stock ticker for Mac?

Yes. MarketPulseBar can display supported stock symbols and market movement directly in the macOS menu bar, while also supporting crypto, ETFs, forex, indices, and commodities.

### Can MarketPulseBar track crypto prices?

Yes. Cryptocurrency symbols supported by Yahoo Finance can be included in your MarketPulseBar watchlist.

### Can I track portfolio profit and loss?

Yes. Portfolio mode lets you enter units and average cost so MarketPulseBar can show the current profit or loss for a tracked position.

### Does it support ETFs and forex?

Yes. MarketPulseBar supports Yahoo Finance symbols for ETFs, forex, indices, and other available instruments in addition to stocks and crypto.

### Does MarketPulseBar support price alerts?

Yes. You can configure price alerts for symbols you care about.

### Does MarketPulseBar place trades?

No. MarketPulseBar is a market-awareness and portfolio-tracking utility. It is not a brokerage and does not replace a trading platform.

### Where does the market data come from?

MarketPulseBar uses Yahoo Finance as its market-data source. Exact coverage and symbol behaviour depend on Yahoo Finance.

### Is MarketPulseBar open source?

No. MarketPulseBar is closed source. This repository exists for product documentation, public release information, bug reports, and feature requests.

---

## Support and feedback

Found a problem or have an idea?

- [Report a bug](../../issues/new?template=bug_report.md)
- [Request a feature](../../issues/new?template=feature_request.md)
- Read [`SUPPORT.md`](SUPPORT.md) before posting sensitive information

For security-related issues, please follow [`SECURITY.md`](SECURITY.md) instead of opening a public issue.

---

## Learn more

- **Product page:** https://mustafaramx.com/apps/marketpulsebar/
- **Build story:** https://mustafaramx.com/post/marketpulsebar-track-crypto-stocks-etfs-gold-silver-p-l-in-your-mac-menu-bar/
- **Video demo:** https://www.youtube.com/watch?v=_PoSTb12ScQ
- **Developer:** https://mustafaramx.com/

---

## Disclaimer

MarketPulseBar is a personal productivity and market-awareness tool, not financial advice.

Market data coverage, availability, freshness, and symbol behaviour depend on Yahoo Finance and the instruments it supports.

---

**MarketPulseBar** · A focused stock, crypto, ETF, forex, commodity, and portfolio tracker for the macOS menu bar.
