GOLD AI TRADER — Android PWA MVP
================================

This is a mobile-first installable web app, not a native APK and not an MT5 Expert Advisor.

What works:
- Fetches indicative XAU/USD spot from XAUS (free public endpoint, no API key).
- Refreshes once per minute.
- Reads XAUS 5-minute sampled intraday points and calculates EMA20, EMA50 and RSI14.
- Displays a basic directional bias only when the indicators agree.
- Shows source status / timestamp and a stale-data warning.
- Does not place trades, connect to MT5, or promise profitable signals.

Data caveats:
- XAUS spot is indicative mid-market data, not the user's broker execution quote.
- The intraday series is sampled every 5 minutes, not broker OHLC candles.
- Indicators are educational heuristics, not a validated trading strategy.
- Use the broker's own XAUUSD quote, spread, contract size and risk settings before any trade.
- API docs: https://xaus.com/api/

Install on Android:
A PWA requires HTTPS hosting to be installable. The ZIP itself is source files, not a directly installable APK.
1. Extract this ZIP.
2. Upload the folder contents to a static HTTPS host (for example GitHub Pages or Netlify).
3. Open the hosted HTTPS address in Chrome on Android.
4. Chrome menu (⋮) > Install app / Add to Home screen.
5. Open from the new home-screen icon.

You can preview index.html in a browser, but file:// preview may block network requests or PWA installation.
