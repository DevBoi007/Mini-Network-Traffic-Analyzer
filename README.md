# Mini Network Traffic Analyzer

A Network traffic capture and analysis CLI tool with protocol distribution, top talkers, and bandwidth visualization.

## What It Does

- Capture live network traffic on any interface with configurable packet counts
- Real-time protocol distribution analysis with percentage breakdowns
- Top talkers identification showing most active IP addresses by traffic volume
- Bandwidth calculation with bytes sent/received per endpoint
- Verbose mode displays individual packet flow with source/destination details
- Built on Scapy for deep packet inspection and protocol parsing

## Quick Start

```bash
uv tool install netanal
sudo netanal capture -i eth0 -c 100
```

> [!TIP]
> This project uses [`just`](https://github.com/casey/just) as a command runner. Type `just` to see all available commands.
>
> Install: `curl -sSf https://just.systems/install.sh | bash -s -- --to ~/.local/bin`

## Commands

| Command | Description |
|---------|-------------|
| `netanal capture` | Live packet capture with protocol analysis, top talkers, and bandwidth stats |
