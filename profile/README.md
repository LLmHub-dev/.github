**LLmHub** is the drop‑in API that decides which Large Language Model should answer each prompt—so you don’t have to. Slash inference bills, speed up responses, and keep full control over quality & privacy.

## ✨ Why LLmHub?

* ⏱️ **Latency-aware routing** – chooses the fastest model available in real‑time.
* 💸 **Cost optimiser** – automatically sends simple prompts to cheaper models, reserving GPT‑4o‑class power for complex tasks.
* 📊 **Transparent analytics** – detailed per‑request breakdowns of tokens, spend and speed.
* 🔒 **Bring‑your‑own‑keys** – your credentials never leave your VPC; works with OpenAI, Anthropic, Mistral, Together AI and more.
* 🧠 **Learning cache** – semantic caching means repeated or similar prompts return instantly at zero cost.
* ⚙️ **Plug‑and‑play SDKs** – first‑class clients for Python, JavaScript/TypeScript and Go.

## 🚀 Quick Start

```bash
pip install llmhub
export LLMHUB_API_KEY="YOUR_KEY"
```

```python
from llmhub import Client

client = Client()
response = client.chat("Summarise the latest AI news in 3 bullet points.")
print(response.text)
```

## 🛠️ Features

| Category                      | What you get                                                              |
| ----------------------------- | ------------------------------------------------------------------------- |
| **Automatic Model Selection** | Real‑time scoring based on price, speed, capacity and historical accuracy |
| **Smart Retry & Fallback**    | If a provider throttles, LLmHub transparently re‑routes the call          |
| **Version Pinning**           | Lock a route to a specific provider/model for compliance needs            |
| **Per‑org Limits**            | Define budgets, rate limits and hard caps in a few clicks                 |

## 🗝️ API Key Management

Generate and rotate API keys from the dashboard or via CLI:

```bash
llmhub keys create "dev-environment"
llmhub keys list
llmhub keys revoke <key_id>
```

Every key is scoped and can be limited by daily spend, QPS or model list.

## 📊 Real‑time Metrics

The dashboard shows:

* Requests per minute & latency percentiles
* Token usage by provider
* Cost heat‑map over time
* Cache hit ratio

## 🤝 Contributing

We love community contributions!  Whether it’s a bug fix, new provider adapter or docs improvement:

1. **Fork** the repo & create a feature branch.
2. **Commit** your changes with clear messages.
3. **Open** a Pull Request.
4. We’ll run CI and help you land it.

See [`CONTRIBUTING.md`](CONTRIBUTING.md) for coding standards & release flow.

## 🛣️ Roadmap

* 🔌 WebSocket streaming responses
* 🛡️ On‑premise “air‑gapped” deployment option
* 📈 Predictive pre‑warm logic for even lower p99 latency

Vote or propose new features in [Discussions](https://github.com/llmhub/llmhub/discussions).

## 📞 Contact

| Channel      | Link                                                                       |
| ------------ | -------------------------------------------------------------------------- |
| 🌐 Website   | [https://llmhub.dev](https://llmhub.dev)                                   |
| ✉️ Email     | [prateek@llmhub.dev](mailto:prateek@llmhub.dev)                            |
| 💼 LinkedIn  | [https://linkedin.com/company/llmhub](https://linkedin.com/company/llmhub) |
| 🐦 Twitter/X | @llmhubdev                                                                 |

## 📝 License

Distributed under the MIT License. See [`LICENSE`](LICENSE) for more information.

---

<p align="center">Made with ❤️ by the LLmHub team</p>
