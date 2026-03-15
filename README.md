# Trading Journal Pro

A professional, fully offline trading journal built as a single HTML file. No installation, no backend, no dependencies. Open the file in any browser and start trading.

Optimised for desktop, Android, and iPhone.

---

## Overview

Trading Journal Pro is a self-contained HTML file — every line of CSS, JavaScript, and markup lives in one place. There is no server, no database, no account, and no internet connection required at any point. Data is stored locally in the browser's localStorage and persists across sessions.

The interface is fully responsive. It adapts to desktop screens with a sidebar and topbar navigation, and switches to a bottom navigation bar with an overlay sidebar on phones and tablets. It has been specifically tested and optimised for iPhone Safari, including safe area insets for the home indicator and notch, 16px input sizing to prevent auto-zoom, and touch-action handling for reliable tap response.

---

## How to Use

Download `TRADING-JOURNAL-PRO.html` and open it in any modern browser. Nothing else is required.

**On iPhone or Android** — the recommended method is to host the file online (see below) and open the URL in Safari or Chrome, then use Add to Home Screen to install it as a standalone app.

**On Desktop** — double-click the file to open it in your default browser, or drag it into any browser window.

---

## Device Support

| Platform | Status |
|----------|--------|
| Desktop (Windows, Mac, Linux) | Fully supported |
| iPhone (Safari) | Fully optimised |
| Android (Chrome) | Fully supported |
| iPad | Fully supported |
| All modern browsers | Fully supported |

The layout automatically adapts based on the device:

- **Desktop** — fixed sidebar, topbar navigation, full multi-column layout
- **Mobile and tablet** — bottom navigation bar, slide-in overlay sidebar, single-column layout, touch-optimised tap targets

---

## Features

### Dashboard
- Equity curve — green when net positive, red when in drawdown
- Daily P&L bar chart
- Key metrics: Net P&L, Win Rate, Profit Factor, Days Traded, Total Trades
- Recent sessions list and performance breakdown

### Journal
- One session per trading day
- Unlimited trades per session
- Chart screenshot uploads with a full lightbox viewer (click to zoom, scroll to zoom, arrow key navigation)
- Per-trade fields: Symbol, Direction, Entry, Exit, Size, Stop Loss, Take Profit, P&L, R:R, Setup, Tags, Notes
- Auto-calculated P&L and R:R from entry/exit/stop fields
- Pre-market preparation notes and end-of-day review
- Emotion tracking across seven states
- Trade quality rating from one to five stars

### Calendar
- Monthly view with colour-coded win and loss days
- P&L displayed per day
- Click any day to navigate directly to that session

### Trade Log
- Complete table of every trade across all sessions
- Colour-coded P&L, direction, and outcome
- Trade count displayed in header

### Statistics
- Equity curve
- Win, Loss, and Breakeven distribution chart
- Daily P&L bar chart
- Setup win rate breakdown
- Monthly P&L trend

### Rules and Plan
- Account details: broker name, account size, type, market, risk percentage, max daily loss
- Trading rules checklist with pass/fail toggle
- Trade setups library
- Full trading plan: pre-market routine, entry criteria, exit criteria, risk management
- Mindset and psychology notes

### Notes
- Free-form notes with title, body, and timestamp
- Sidebar list for quick navigation between notes
- Separate from the trade journal

---

## Customisation

All settings are accessible from the Settings panel in the top right.

- **Account** — upload a custom logo image, set journal name and subtitle, set logo initials as fallback
- **Theme** — dark and light mode
- **Glow Effects** — toggle neon glow on or off. When off, the interface becomes clean and flat. When on, dark mode includes neon text shadows, scanlines, and a dot-grid background
- **Accent Colour** — full HSV colour picker with a saturation/brightness gradient, hue slider, hex input field, and twelve preset swatches. Applied instantly across the entire interface
- **Compact Mode** — reduces padding and spacing for smaller screens

---

## Data and Privacy

All data is stored in the browser's localStorage on your device. Nothing is sent anywhere.

- No account or login required
- No tracking, analytics, or telemetry of any kind
- No internet connection required after the file is loaded
- Fully functional offline

**Export** — saves all sessions, trades, rules, account details, and branding as a `.json` file. Use this to back up your data or move it to another device.

**Import** — restores a previously exported `.json` file. All existing data will be replaced.

---

## Hosting on iPhone (Recommended Method)

Because iPhone Safari restricts local HTML files, the most reliable way to use this on iPhone is to host it online and open the URL in Safari.

**Netlify Drop** (free, no account needed):
1. Go to [netlify.com/drop](https://netlify.com/drop)
2. Drag and drop the HTML file onto the page
3. Copy the generated URL
4. Open the URL on your iPhone in Safari
5. Tap Share → Add to Home Screen

The app will appear on your home screen and open fullscreen with no browser chrome, identical to a native app.

Other free hosting options: GitHub Pages, Tiiny.host, Vercel.

---

## Data Persistence Across Devices

Because data is stored in localStorage, it is tied to the browser on each device. Data on your iPhone does not automatically sync to your desktop and vice versa.

To move data between devices:
1. On the source device, open Settings → Export → save the `.json` file
2. Transfer the file to the target device (email, AirDrop, iCloud, WhatsApp)
3. On the target device, open Settings → Import → select the `.json` file

---

## File Structure

The entire application is a single file:

```
TRADING-JOURNAL-PRO.html
```

It contains no external dependencies. All fonts use system font stacks. All charts are drawn using the HTML Canvas 2D API. No CDN scripts are loaded.

---

## Browser Compatibility

| Browser | Support |
|---------|---------|
| Chrome 90+ | Full |
| Safari 14+ (iOS and macOS) | Full |
| Firefox 90+ | Full |
| Edge 90+ | Full |
| Samsung Internet | Full |

---

## Roadmap

- Cloud sync via self-hosted backend
- CSV export for spreadsheet analysis
- Broker API integration for automatic trade import
- Weekly and monthly review templates
- Risk and position size calculator

---

## License

MIT License. Free to use, modify, and distribute.
