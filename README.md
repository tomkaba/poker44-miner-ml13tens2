# Poker44-gen13tens1

Minimal release repository for Poker44 miner runtime scoring.

This repository is a standalone miner variant prepared for production rollout.

## Quick start

```bash
git clone https://github.com/tomkaba/poker44-miner-gen13tens1.git
cd poker44-miner-gen13tens1
python3 -m venv .venv
source .venv/bin/activate
pip install -r requirements.txt
pip install -e .
```

## Run Miner

```bash
python neurons/miner.py
```

or legacy wrapper:

```bash
./start_miner.sh HOTKEY_ID[,HOTKEY_ID2,...]
```

## Implementation

- Scorer entrypoint: poker44/miner_heuristics.py
- Entry point: neurons/miner.py

Manifest implementation SHA256 is computed from:

- neurons/miner.py
- poker44/miner_heuristics.py
- runtime files tracked in repository
