# BTCRecover Setup Guide

## Requirements
- Python 3.9+
- pip

## Install
```bash
git clone https://github.com/3rdIteration/btcrecover.git
cd btcrecover
pip install -r requirements.txt
```

## Recover Wallet Password
```bash
python btcrecover.py --wallet wallet.dat \
  --passwordlist wordlist.txt
```

## Recover Seed Phrase
```bash
python seedrecover.py --wallet-type bitcoin \
  --addrs YOUR_BTC_ADDRESS
```

## Useful Flags
```
--typos 2          # try 2 typos per guess
--typos-swap       # swap character pairs
--typos-case       # try case variations
--max-tokens 12    # limit seed words checked
```

## Wordlist tip
Use `rockyou.txt` or build a custom list of
passwords you likely used.

## Docs
👉 https://btcrecover.readthedocs.io

> ⚠️ **Legal use only** — only attempt recovery on wallets you own.
