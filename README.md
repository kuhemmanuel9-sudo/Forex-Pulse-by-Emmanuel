# Forex Pulse

Forex Pulse is a foreign exchange analytics and decision support dashboard designed and developed by Emmanuel Kuh. It combines currency conversion, market monitoring, historical trends, risk analytics, currency strength, market sessions, and browser voice briefings in one clean single-file app.

I built this as a portfolio project to show practical front end engineering, financial data integration, accessible interface design, charting, browser speech, and transparent JavaScript analytics.

## What It Does

Forex Pulse helps users monitor currency pairs and understand market conditions from recent exchange-rate data. It does not tell people what to trade; it presents rates, movement, volatility, drawdown, risk, and momentum so users can interpret the market for research and education.

The dashboard runs as a single HTML file. It does not require a backend, database, account, or paid API key.

## Features

1. Global currency converter
2. Major forex pair watchlist
3. Custom pair builder
4. Free no-key reference-rate data
5. Live FX mode where the free source supports it
6. Historical pair chart with calendar-aware 7D, 30D, 90D, and 1Y ranges
7. Momentum score
8. Risk score
9. Volatility and drawdown estimates
10. Seven-day and thirty-day movement
11. Currency strength heatmap
12. World trading session monitor
13. Voice market briefing
14. Installed browser voice selector
15. Beginner mode with plain-English pair explanations
16. Forex basics glossary
17. Dark and light themes
18. Dedicated mobile summary view
19. Local storage for saved pairs and settings
20. Transparent methodology modal

## Built With

1. HTML
2. CSS
3. JavaScript
4. Frankfurter API
5. exchangerate.dev API
6. Chart.js
7. Lucide icons

## Data Sources

Reference rates come from Frankfurter, a free exchange-rate API that uses institutional and central-bank sources.

Live mode uses exchangerate.dev where available. If live data cannot be reached, the dashboard falls back to Frankfurter reference rates.

Rates are indicative and are not dealing quotes.

## How The Scores Work

The momentum score uses recent movement, trend consistency, and broader context, then reduces the score when market risk is elevated.

The risk score uses recent volatility, drawdown from the recent high, and unusually large one-day movement to identify unstable conditions. The period calculations locate the nearest prior available observation to the target calendar date, which avoids treating missing weekend or holiday data as if it were a normal trading day.

These calculations are intentionally transparent. They are designed to describe market conditions, not to promise returns.

## Beginner Mode

Forex Pulse includes a plain-English layer for people who are new to forex. It explains what a pair means, what the exchange rate means, whether the base or quote currency appears stronger, and why the dashboard score should be treated as an educational indicator instead of a buy or sell instruction.

## How To Run It

Open `forex-trading-dashboard.html` in a modern browser.

No build step is required. The HTML, CSS, and JavaScript are all included in one file.

## Important Note

Forex Pulse is for research, education, and portfolio demonstration. It does not provide financial advice, does not place trades, and does not guarantee profit or returns.

## Author

Designed and Developed by Emmanuel Kuh.
