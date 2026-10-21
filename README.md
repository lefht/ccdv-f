# ccdv-f

A minimal example of the [Claude Agent SDK](https://docs.claude.com/en/docs/agent-sdk/overview) for Python. `agent.py` asks Claude how many files are in the current directory and prints the answer. Claude can only use the read-only tools `Read`, `Glob` and `Grep`.

## Requirements

- Python 3.10+
- An Anthropic API key

## Setup

```bash
python -m venv .venv
source .venv/bin/activate
pip install claude-agent-sdk
export ANTHROPIC_API_KEY=your-key-here
```

## Usage

```bash
python agent.py
```

To ask something else, change the `prompt` in `agent.py`. To give Claude more tools, edit `allowed_tools`.
