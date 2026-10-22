# LMCache on CPU: with and without

A notebook that runs two copies of vLLM on your CPU, one plain and one backed by
LMCache, loads a long document into LMCache, and lets you ask questions in a
side-by-side UI to compare time to first token. No GPU.

## Before you start

Python 3.12 is required.

| | |
|---|---|
| macOS | `brew install python@3.12 ffmpeg` |
| Ubuntu 24.04, x86_64 | `sudo apt install python3.12-venv python3.12-dev libnuma1 ffmpeg` |

## Start the notebook

```bash
git clone git@github.com:sammshen/lmcache-cpu-demo.git
cd lmcache-cpu-demo
python3.12 -m venv .venv
source .venv/bin/activate
pip install jupyterlab
jupyter lab LMCache_CPU_Demo.ipynb
```

Run the cells top to bottom.
