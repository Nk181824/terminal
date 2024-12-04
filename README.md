import mplfinance as mpf
import pandas as pd

# Sample data
dates = pd.date_range(start="2023-01-01", periods=30, freq="D")
prices = {
    "Open": [1.1, 1.12, 1.11, 1.13, 1.15, 1.14, 1.13, 1.16, 1.18, 1.19, 1.17, 1.16, 1.14, 1.15, 1.13, 1.12, 1.1, 1.08, 1.1, 1.09, 1.11, 1.12, 1.1, 1.09, 1.11, 1.12, 1.13, 1.14, 1.16, 1.15],
    "High": [1.12, 1.13, 1.12, 1.15, 1.16, 1.15, 1.14, 1.18, 1.19, 1.2, 1.18, 1.17, 1.15, 1.16, 1.14, 1.13, 1.12, 1.1, 1.12, 1.1, 1.12, 1.13, 1.12, 1.1, 1.12, 1.14, 1.15, 1.16, 1.18, 1.17],
    "Low": [1.08, 1.1, 1.09, 1.12, 1.13, 1.12, 1.12, 1.14, 1.17, 1.18, 1.15, 1.14, 1.12, 1.13, 1.12, 1.11, 1.08, 1.07, 1.09, 1.07, 1.1, 1.1, 1.08, 1.07, 1.1, 1.11, 1.12, 1.14, 1.15, 1.14],
    "Close": [1.11, 1.12, 1.1, 1.14, 1.15, 1.13, 1.13, 1.17, 1.18, 1.19, 1.16, 1.15, 1.13, 1.14, 1.12, 1.11, 1.09, 1.08, 1.1, 1.09, 1.11, 1.11, 1.09, 1.08, 1.11, 1.12, 1.13, 1.15, 1.16, 1.16],
}
df = pd.DataFrame(prices, index=dates)

# Plot candlestick chart
mpf.plot(
    df,
    type="candle",
    title="Japanese Candlestick Chart Example",
    ylabel="Price",
    style="yahoo",
)
```

## Themes

![themes](/docs/screenshot.gif)

[Here's](/docs/themes) a list of available themes.


## Contributing

Please feel free to pull requests or log issues.

Thanks!

## Star History

[![Star History Chart](https://api.star-history.com/svg?repos=m4tt72/terminal&type=Date)](https://star-history.com/#m4tt72/terminal&Date)
