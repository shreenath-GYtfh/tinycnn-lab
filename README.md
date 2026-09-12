# tinycnn-lab

Minimal training loop I use to test ideas fast

## Examples

```bash
python train.py --epochs 5 --synthetic
# metrics land in runs/metrics.csv
```

## What it does

- Cosine LR schedule with warmup
- Single file model definition, easy to hack
- Gradient clipping and clean metrics logging
- Synthetic dataset mode: no download needed to smoke-test
- Metrics logged to CSV for plotting

## Installation

```bash
pip install -r requirements.txt
```

## Project structure

```text
├── .github/
│   └── workflows/
│       └── ci.yml
├── docs/
│   └── development.md
├── examples/
│   └── quickstart.md
├── .gitattributes
├── .gitignore
├── CHANGELOG.md
├── CONTRIBUTING.md
├── SECURITY.md
├── model.py
├── requirements.txt
└── train.py
```

## Development

```bash
python -m venv .venv && source .venv/bin/activate
pip install -r requirements.txt
```
