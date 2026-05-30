## Jan Hilgard — AI inference engineer, serial founder

I build systems for running large language models efficiently on local hardware. Currently focused on inference engine optimization for Apple Silicon — specifically M3 Ultra deployments, MLX quantization (Q6/Q8), KV cache strategies, and agentic pipelines that actually work in production.

I'm a co-founder and CTO in the AI space. Before that, I founded and ran Hosting90, a Czech hosting and cloud infrastructure company, for 18 years before exiting in 2020. That background in running infrastructure at scale informs how I think about LLM serving: reliability, latency, and resource efficiency matter more than benchmark headlines.

### What I'm working on

- **vllm-mlx** — Core contributor to [vllm-mlx](https://github.com/waybarrios/vllm-mlx) (80+ PRs; second external contributor by join order), an OpenAI-compatible inference server built on MLX for Apple Silicon. Specific contributions:
  - **MTP speculative decoding for Qwen3-Next** ([PR #82](https://github.com/waybarrios/vllm-mlx/pull/82), merged) — Multi-Token Prediction with always-advance strategy and rejection sampling; 1.43x verified / 1.76x optimistic on M3 Ultra
  - **Draft-model speculative decoding** ([PR #45](https://github.com/waybarrios/vllm-mlx/pull/45), merged) — HybridEngine sharing a single model instance across speculative and batched modes; 1.2–1.4x throughput improvement
  - Prefix caching, KV cache quantization, Anthropic Messages API integration, MoE model support
  - Assigned collaborator on [MTP roadmap for Qwen3-Next / MiMo / Qwen3.5 family](https://github.com/waybarrios/vllm-mlx/issues/56) alongside the repo owner
- **vllm-mlx-dashboard** — Real-time monitoring dashboard for local LLM inference servers (llama.cpp + vllm-mlx), built with Next.js.
- M3 Ultra (256 GB) benchmarking — sustained throughput, quantization tradeoffs, batch size effects at the edge of consumer hardware.

### Background

- 2020–present: Co-founder & CTO, AI inference tooling
- 2002–2020: Founder & CEO, Hosting90 (Czech hosting/cloud, exited)
- Focus areas: inference optimization, local LLM deployment, agentic systems

### Tech I work with

`Python` `TypeScript` `MLX` `vLLM` `Next.js` `Apple Silicon` `llama.cpp` `KV cache` `quantization`

### Reach me

- [hilgard.cz](https://hilgard.cz)
- [linkedin.com/in/janhilgard](https://linkedin.com/in/janhilgard)
