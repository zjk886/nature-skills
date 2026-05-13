# Model Providers

Use this skill with official provider APIs. Keep the paper-reader contract provider-neutral and only swap the backend configuration.

## Supported official APIs

| Provider | Official base URL | Notes |
|---|---|---|
| DeepSeek | `https://api.deepseek.com` | Official OpenAI-compatible API. |
| GLM / Zhipu | `https://open.bigmodel.cn/api/paas/v4` | Official OpenAI-compatible API. |
| Qwen / DashScope | `https://dashscope.aliyuncs.com/compatible-mode/v1` | Official OpenAI-compatible API. |
| Kimi / Moonshot | `https://api.moonshot.cn/v1` | Official OpenAI-compatible API. |

## Practical rule

Use the same request shape everywhere:

- `base_url`
- `api_key`
- `model`
- chat messages or tool calls

Do not hardcode provider-specific prompt wrappers into the skill. Keep the paper workflow the same and move only the transport layer behind the provider adapter.

## Examples

- Use DeepSeek when the user already has a DeepSeek account or wants DeepSeek reasoning models.
- Use GLM when the user already has a BigModel/Zhipu account.
- Use Qwen when the user already has an Alibaba Cloud/DashScope account.
- Use Kimi when the user already has a Moonshot account.

## Selection guidance

If the user does not care which provider is used, pick the one already configured in the project. If nothing is configured, ask for a provider rather than guessing credentials or mixing unofficial endpoints.
