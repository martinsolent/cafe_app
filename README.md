# The Little Bean Café – Owner Dashboard Prototype

A clickable, high-fidelity prototype for **UX testing**. It shows how a small café owner could check how the day is going at a glance on a laptop, between serving customers. All data is made up and nothing is saved.

## Purpose

To test whether an independent café owner can complete this main task without help:

> Find out which item sold best yesterday, then see which items are running low on stock.

## Key features

The prototype has four screens:

1. **Overview** – today's sales, number of orders and the busiest hour, with shortcuts to best sellers and stock levels.
2. **Sales by item** – all 20 menu items for yesterday, today so far or the last 7 days. The table can be sorted and searched, and a simple bar chart sits beside it. The best seller is named at the top.
3. **Item details** – the last 7 days of units and revenue for one item, with a small bar chart and its current stock status. A back button returns to the screen you came from.
4. **Stock levels** – every item with stock remaining, a reorder level and an estimate of days left. Low-stock items are flagged with an icon and text (not colour alone) and listed first. A "Low stock only" filter can be switched on and off.

Other behaviour:

- **Unbuilt areas** (Reports, Settings, Help, Create reorder list) show the message "This part isn't in the prototype yet."
- **Mistakes can be corrected**: you can go back, clear the search, change the sort, or untick the filter.
- **Reset prototype** (footer link) returns to the first screen and clears everything entered, so each test session starts cleanly.
- **Realistic content**: 20 coffees, teas, cakes and sandwiches in UK English, with 7 days of generated sales and stock figures in pounds.

## Design and accessibility

- Built with Google **Material Web components (Material 3)**, with a coffee-brown accent colour. Custom CSS is limited to small layout adjustments.
- Semantic HTML, a label on every input, visible keyboard focus, a logical heading order and a skip link.
- Colours chosen for WCAG 2.2 AA contrast; light and dark modes are supported.
- Designed for a laptop (about 1280px wide) and stacks neatly on a phone.

## Files

| File | Description |
| --- | --- |
| `cafe-dashboard.html` | The whole prototype: HTML, CSS and JavaScript in one file. Screen sections are marked with comments (`SCREEN 1` to `SCREEN 4`). |
| `README.md` | This description. |

The only external files are the Material Web library (from jsDelivr) and the Roboto font (from Google Fonts). There is no server, database, login or real API.

## How to run it

Open `cafe-dashboard.html` in a modern browser with an internet connection (needed to load Material Web). No installation is required.

## Limitations

- Sales and stock figures are generated from fixed patterns, not real café data.
- Nothing is stored; refreshing the page or choosing "Reset prototype" returns everything to the start.
