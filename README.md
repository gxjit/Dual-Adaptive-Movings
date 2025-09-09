### Dual Adaptive Movings 
By Gurjit Singh

A dual-layer adaptive moving average system that adjusts its responsiveness dynamically using market-derived factors (CMO, RSI, Fractal Roughness, or Stochastic Acceleration). It plots:

* Primary Adaptive MA (MA): Fast, reacts to changes in volatility/momentum.
* Following Adaptive MA (FAMA): A smoother, half-alpha version for trend confirmation.

Instead of fixed smoothing, it adapts dynamically using one of four methods:

* ACMO: Adaptive CMO (momentum)
* ARSI: Adaptive RSI (relative strength)
* FRMA: Fractal Roughness (volatility + fractal dimension)
* ASTA: Adaptive Stochastic Acceleration (%K acceleration)

### ⚙️ Inputs & Options

* Source: Price input (default: close).
* Moving (Type): ACMO, ARSI, FRMA, ASTA.
* MA Length (Primary): Core adaptive window.
* Following (FAMA) Length: Optional; can match MA length.
* Use Wilder’s: Toggles Wilder vs EMA-style smoothing.
* Colors & Fill: Bullish/Bearish tones with transparency control.

### 🔑 How to Use

1. Identify Trend:
   * When MA > FAMA → Bullish (fills bullish color).
   * When MA < FAMA → Bearish (fills bearish color).

2. Crossovers:
   * MA crosses above FAMA → Bullish signal 🐂
   * MA crosses below FAMA → Bearish signal 🐻
   
3. Adaptive Edge:
   * Select method (ACMO/ARSI/FRMA/ASTA) depending on whether you want sensitivity to momentum, strength, volatility, or acceleration.
   
4. Alerts:
   * Built-in alerts trigger on crossovers.

#### 💡 Tips

* Wilder’s smoothing is gentler than EMA, reducing whipsaws in sideways conditions.
* ACMO and ARSI are best for momentum-driven directional markets, but may false-signal in ranges.
* FRMA and ASTA excels in choppy markets where volatility clusters.

👉 In short: Dual Adaptive Movings adapts moving averages to the market’s own behavior, smoothing noise yet staying responsive. Crossovers mark possible trend shifts, while color fills highlight bias.
