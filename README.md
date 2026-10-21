# proxy_rules
Proxy rules

## AI 服务规则

规则位于 `surge-rules/`，使用 Surge 规则列表格式。

| 文件 | 服务 |
| --- | --- |
| `claude.list` | Claude / Anthropic |
| `openai.list` | OpenAI / ChatGPT / Sora / Codex |
| `gemini.list` | Google Gemini |
| `appleIntelligence.list` | Apple Intelligence |
| `augmentCode.list` | AugmentCode |
| `cursor.list` | Cursor |
| `xai.list` | X / Twitter / Grok / xAI |
| `meta.list` | Meta / Facebook / Instagram / WhatsApp 等 |
| `muse.list` | Muse / Llama / Meta AI |
| `trae.list` | Trae |
| `windsurf.list` | Windsurf / Codeium |
| `other-ai.list` | OpenRouter / Poe |

2026-10-21 根据 `jinxinkai/clash-ai-rules` 的 `81e4f7a` 快照补齐规则，保留本地已有扩展。

- 上游的 `DOMAIN-REGEX` 规则由 `DOMAIN-KEYWORD,chatgpt` 覆盖，不直接写入 Surge 列表。
- `grok.com`、`x.ai` 为额外补充，不在该上游快照中。
- `meta.list` 覆盖大量非 AI 服务；启用后，这些服务也会匹配对应的分流策略。
- 新增的列表需要在实际 Surge 配置中引用后才会生效。
