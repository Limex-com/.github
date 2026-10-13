# ZIPLIME by Limex

**Open-source backtesting and live trading. Zipline reborn on Polars, built for the age of AI.**

Describe a strategy in plain English or write it in Python. ZIPLIME backtests it in seconds on point-in-time data, shows you what actually drove the returns, and takes it live when you're ready.

[**Get started**](https://github.com/Limex-com/ziplime) · [**Web app**](https://ziplime.limex.com/home) · [**Datasets**](https://huggingface.co/ZipLime) · [**Discussions**](https://github.com/Limex-com/ziplime/discussions)

---

## Why ZIPLIME

Zipline was the standard for Python backtesting until it was abandoned, stuck on legacy pandas and Python 3.6. ZIPLIME keeps the API quants already know and rebuilds everything underneath.

AI made writing strategies easy. It also made it easy to fool yourself: a backtest written by a coding agent looks convincing whether it's right or not. ZIPLIME is built around both halves of that problem: an engine you can trust, and a community of people who know markets and can tell you whether your idea holds up.

## The ecosystem

| Project | What it does |
|---|---|
| [**ziplime**](https://github.com/Limex-com/ziplime) | The core engine. Zipline-compatible API on a Polars data layer. Stocks, ETFs, futures. From backtest to live trading with one flag. Native MCP server for Claude, ChatGPT, Codex, Cursor and other AI clients. |
| [**zipfolio**](https://github.com/Limex-com/zipfolio) | Tearsheets that read the book, not just the returns: positions, instruments, sectors, factor exposures, execution realism, trading costs. Built on pyfolio. |
| [**ZIPLIME on Hugging Face**](https://huggingface.co/ZipLime) | Open point-in-time datasets, packaged as ready-to-ingest ZIPLIME bundles. |
| [**ZIPLIME Web**](https://ziplime.limex.com/home) | The hosted version: AI chat and strategy editor, professional market data, hosted MCP. Nothing to install. |

## Quick start

```bash
pip install ziplime

# backtest
python -m ziplime run -f my_strategy.py --start-date 2023-01-01 --end-date 2023-12-31

# same strategy, live
python -m ziplime run -f my_strategy.py --mode live
```

Full guide and examples in the [ziplime README](https://github.com/Limex-com/ziplime).

## Community

What we missed most about Quantopian wasn't the engine. It was the forums: a place to post a strategy and hear from people who've traded it.

[**GitHub Discussions**](https://github.com/Limex-com/ziplime/discussions) is that place for ZIPLIME. Share strategies, ask why a backtest looks too good, get feedback from practitioners. Strategies built in the open-source engine and in ZIPLIME Web are both welcome.

Found a bug or want a feature? [Open an issue](https://github.com/Limex-com/ziplime/issues).

## Contributing

Pull requests are welcome: engine improvements, data bundles, example strategies, docs. Start with an issue or a discussion so we can help you scope it.

---

<details>
<summary><b>Limex DataHub (legacy tools)</b></summary>

Earlier tools for working with Limex DataHub data are still available:

- [AlgoTrading](https://github.com/Limex-com/AlgoTrading): Jupyter notebooks with example strategies
- [limexhub-python](https://github.com/Limex-com/limexhub-python) and [limexhub-r](https://github.com/Limex-com/limexhub-r): DataHub client libraries
- [Issues](https://github.com/Limex-com/-Issues-): DataHub bug tracker

More at [datahub.limex.com](https://datahub.limex.com/).

</details>

<sub>Made by [Limex](https://limex.com/) · datahub@limex.com</sub>
