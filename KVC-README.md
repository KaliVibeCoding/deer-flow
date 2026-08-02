<!-- KVC Brand Header -->
<div align="center">
<img src="https://cdn.abacus.ai/images/134ce4b7-b0d1-4ba8-8655-3afd323fb646.png" width="64" height="64"/>

# KVC DeerFlow
### by KaliVibeCoding

**AI research and deep-search workflows — KVC branded.**
Kimi 3 leads the research chain. Cloudflare Workers deliver the results.

`Build once. Systemize forever.`
</div>

## KVC Research Model Config

```python
# Primary research orchestrator — Kimi 3 (128K context)
KVC_RESEARCH_LLM = {
    "model": "moonshot-v1-128k",
    "base_url": "https://api.moonshot.cn/v1",
    "api_key": os.environ["MOONSHOT_API_KEY"],
    "temperature": 0.3,  # Lower for research accuracy
}

# Free fallback — Cloudflare edge
KVC_EDGE_LLM = {
    "model": "@cf/meta/llama-3.3-70b-instruct-fp8-fast",
    "base_url": "https://api.cloudflare.com/client/v4/accounts/9a3c0d0f1bc8bb5c83574905b6e13680/ai/v1",
    "api_key": os.environ["CF_AI_API_TOKEN"],
}
```

Apply brand: add `kvc-brand.css` to `web/src/assets/`.
