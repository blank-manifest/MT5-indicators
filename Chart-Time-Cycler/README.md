# Chart Time Cycler

A keyboard shortcut utility indicator for MetaTrader 5. Lets you switch symbols and change timeframes without touching the mouse — using arrow keys and typed numbers directly on the chart.

---

## Features

- **Arrow key symbol switching** — cycle through your Market Watch list with UP / DOWN keys
- **Type-to-change timeframe** — type any MT5 timeframe number and press Enter to switch instantly
- Timeout clears the typed input after N seconds of inactivity
- Shows the typed number on the chart as you type (using MT5 Comment)

---

## How to use

### Switch symbols
- Press **↑ (UP arrow)** — previous symbol in Market Watch
- Press **↓ (DOWN arrow)** — next symbol in Market Watch

Cycles through only the symbols currently in your Market Watch list.

### Change timeframe by typing
Type the timeframe period number directly on the chart and press **Enter**:

| Type | Timeframe |
|---|---|
| `1` | M1 |
| `2` | M2 |
| `3` | M3 |
| `4` | M4 |
| `5` | M5 |
| `6` | M6 |
| `10` | M10 |
| `12` | M12 |
| `15` | M15 |
| `20` | M20 |
| `30` | M30 |
| `60` | H1 |
| `120` | H2 |
| `240` | H4 |
| `1440` | D1 |
| `10080` | W1 |
| `43200` | MN1 |

Press **ESC** to clear what you've typed without switching.

---

## Default Parameters

| Parameter | Default | Description |
|---|---|---|
| Enable symbol switching | `true` | UP/DOWN arrow key symbol cycling |
| Previous symbol key | `38` | Key code for UP arrow |
| Next symbol key | `40` | Key code for DOWN arrow |
| Enable TF typing | `true` | Type number + Enter to change timeframe |
| Confirm key | `13` | Enter key to confirm |
| Clear key | `27` | ESC key to cancel typed input |
| Max digits | `5` | Max length of typed number |
| Timeout (seconds) | `5` | Auto-clear typed input after idle (0 = never) |
| Show typed number | `true` | Display typed digits on chart |

---

## Install

1. Copy `chart_time_cycler.ex5` to your MT5 data folder: **File → Open Data Folder → MQL5 → Indicators**
2. Restart MT5 or right-click Navigator → Refresh
3. Attach to **one chart** — it works globally across all charts from that single instance

> Only attach to one chart at a time. Multiple instances will conflict on key events.

---

> Compiled `.ex5` only — source not included.
