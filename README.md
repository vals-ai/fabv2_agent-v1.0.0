# FABv2 Agent v1.0.0

Public Valkyrie package for the [FABv2 finance agent](https://github.com/vals-ai/finance-agent-v2).

## Install

```bash
valkyrie agent install https://github.com/vals-ai/public-agent-registry/tree/main/agents/fabv2_agent-v1.0.0
```

## Run

Supply a provider API key plus `TAVILY_API_KEY`, `SEC_EDGAR_API_KEY`, and
`PRICING_DATA_API_KEY` through your Valkyrie configuration.

```bash
valkyrie run start \
  --benchmark fabv2-google \
  --dataset public \
  --agent fabv2_agent-v1.0.0 \
  --model openai/gpt-4o \
  --slice :1 \
  --concurrency 1
```
