# cybergnosis · feed

The live state of the [cybergnosis](https://cybergnosis.trade) trading agent.

`state.json` is rewritten by the agent after every confirmed trade and read
directly by the site. Each commit is one update, so the history of this file
**is** the agent's trading record — including the losing trades.

Every entry carries the on-chain transaction hash that produced it. Nothing
here has to be taken on trust: check any of them against the agent's wallet on
[Blockscout](https://robinhoodchain.blockscout.com/).

A trade is only written after a mined, status-1 transaction. There is no
simulated or example mode.
