<div align="center">

<a href="https://kirantallapragada.com">
<picture>
  <source media="(prefers-color-scheme: dark)" srcset="assets/hero-dark.svg">
  <source media="(prefers-color-scheme: light)" srcset="assets/hero-light.svg">
  <img src="assets/hero-dark.svg" width="100%" alt="Kiran Tallapragada, AI and platform architect. I help teams run open LLMs on their own GPUs. Qwen3-8B on one NVIDIA L40S, measured with vLLM 0.31: 15.3 GiB weights, 24.1 GiB KV cache, 175,696 tokens.">
</picture>
</a>

[![Website](https://img.shields.io/badge/WEBSITE-0B0F17?style=for-the-badge&logo=googlechrome&logoColor=F5B942)](https://kirantallapragada.com)
[![Calculator](https://img.shields.io/badge/GPU%20CALCULATOR-F5B942?style=for-the-badge&logo=nvidia&logoColor=0B0F17)](https://kirantallapragada.com/gpu-fit/)
[![LinkedIn](https://img.shields.io/badge/LINKEDIN-0B0F17?style=for-the-badge&logo=linkedin&logoColor=F5B942)](https://www.linkedin.com/in/kiran-tallapragada/)
[![Medium](https://img.shields.io/badge/MEDIUM-0B0F17?style=for-the-badge&logo=medium&logoColor=F5B942)](https://medium.com/@tallapragada.kiran)
[![RSS](https://img.shields.io/badge/RSS-0B0F17?style=for-the-badge&logo=rss&logoColor=F5B942)](https://kirantallapragada.com/subscribe/)

</div>

### What I do

**Since 2024, CTO:** took AI products from one market to several, including a new international market, and built the 55+ engineering organisation (in-house and partner teams) behind them. **2018 – 2024, global pharma:** Manager to Lead Architect at Associate Director level.

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="assets/cards-dark.svg">
  <source media="(prefers-color-scheme: light)" srcset="assets/cards-light.svg">
  <img src="assets/cards-dark.svg" width="100%" alt="Run: self-hosted LLMs on vLLM (H100, L40, L40S), AWQ and FP8, shared-GPU budgets, admission control, recovery when a GPU drops out. Read: document AI for financial and regulatory filings, structured output, LLM gateways with per-call token and cost tracking. Build: cloud platforms on AWS end to end: multi-account, networking and security, GPU fleets and CI/CD, designed to be audited.">
</picture>

### gpu-fit: will this model fit on this GPU?

Weights, runtime overhead and KV cache, the way vLLM actually allocates them, then a `vllm serve`
command that starts. [Repository](https://github.com/KiranTallapragada/gpu-fit) ·
[PyPI](https://pypi.org/project/gpu-fit/) · [browser calculator](https://kirantallapragada.com/gpu-fit/)

<a href="https://github.com/KiranTallapragada/gpu-fit">
<img src="assets/terminal.svg" width="100%" alt="Terminal: pip install gpu-fit, then gpu-fit sizes Qwen3-8B-FP8 on an NVIDIA L4 at 32K context with an FP8 KV cache: 20.7 GiB budget, 8.8 GiB weights, 2.0 GiB overhead, 9.9 GiB KV cache, 144,558 tokens, 4.4 full requests, fits.">
</a>

### Checked against real GPUs

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="assets/accuracy-dark.svg">
  <source media="(prefers-color-scheme: light)" srcset="assets/accuracy-light.svg">
  <img src="assets/accuracy-dark.svg" width="100%" alt="gpu-fit's KV-cache prediction against what vLLM 0.31 allocated, 16 runs on L40S, A10G and L4. Dense models with the default KV cache: within 0.5%. FP8 KV cache and 16K context: up to 9% cautious. Hybrid MoE model: 11.6% cautious.">
</picture>

<sub>Raw data and method: [gpu-fit/bench](https://github.com/KiranTallapragada/gpu-fit/tree/main/bench) · full table: [accuracy, measured](https://github.com/KiranTallapragada/gpu-fit#accuracy-measured)</sub>

### Building in the open

| Project | What it answers | |
|---|---|---|
| [**gpu-fit**](https://github.com/KiranTallapragada/gpu-fit) | Will this LLM fit on this GPU, how much context, how many users, and what if the GPU is shared? | [![PyPI](https://img.shields.io/pypi/v/gpu-fit?style=flat-square&color=F5B942&labelColor=0B0F17)](https://pypi.org/project/gpu-fit/) |
| [**gpu-guard**](https://github.com/KiranTallapragada/gpu-guard) *(new)* | Is your self-hosted LLM really on the GPU? A health check that catches silent CPU fallback, for vLLM, Ollama or any OpenAI-compatible server. | ![Go](https://img.shields.io/badge/Go-0B0F17?style=flat-square&logo=go&logoColor=00ADD8) |

### Stack

<p>
<img src="https://skillicons.dev/icons?i=py,go,rust,ts,bash,aws,docker,linux,postgres,redis,nestjs,githubactions,cloudflare&perline=14" width="100%" alt="Python, Go, Rust, TypeScript, Bash, AWS, Docker, Linux, PostgreSQL, Redis, NestJS, GitHub Actions, Cloudflare">
</p>

![vLLM](https://img.shields.io/badge/vLLM-1F5FBF?style=flat-square&logo=vllm&logoColor=white)
![NVIDIA CUDA](https://img.shields.io/badge/NVIDIA%20CUDA-4A7300?style=flat-square&logo=nvidia&logoColor=white)
![Hugging Face](https://img.shields.io/badge/Hugging%20Face-FFD21E?style=flat-square&logo=huggingface&logoColor=black)

### Latest writing

<!-- BLOG-POST-LIST:START -->
- [What fits on a 24 GB GPU: measured on an A10G and an L4](https://kirantallapragada.com/2026/11/what-fits-on-a-24gb-gpu/)
- [A 32B model on a 48 GB GPU: what actually fits](https://kirantallapragada.com/2026/11/a-32b-model-on-a-48gb-gpu/)
<!-- BLOG-POST-LIST:END -->

<sub>Artwork is generated from measured data. Personal work: examples use public models and public data, with no employer or client names or confidential information. Views are my own.</sub>
