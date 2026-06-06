# Awesome Free Models [![Awesome](https://awesome.re/badge-flat.svg)](https://awesome.re)

> A curated list of free AI models, APIs, and tools you can use without paying a cent.

Running AI shouldn't require a credit card. This list curates genuinely free models — open-weight models you can self-host, free API tiers from major providers, and tools to run everything locally.

## Contents

- [Open-Weight Models](#open-weight-models)
  - [Llama Family (Meta)](#llama-family-meta)
  - [Qwen Family (Alibaba)](#qwen-family-alibaba)
  - [Mistral Family](#mistral-family)
  - [DeepSeek Family](#deepseek-family)
  - [Gemma Family (Google)](#gemma-family-google)
  - [Phi Family (Microsoft)](#phi-family-microsoft)
  - [Other Notable Models](#other-notable-models)
- [Free API Providers](#free-api-providers)
- [Local Inference Tools](#local-inference-tools)
- [Multimodal & Vision Models](#multimodal--vision-models)
- [Code Models](#code-models)
- [Embedding Models](#embedding-models)
- [Image Generation Models](#image-generation-models)
- [Audio & Speech Models](#audio--speech-models)
- [Fine-tuning Tools](#fine-tuning-tools)
- [Model Hosting Platforms](#model-hosting-platforms)
- [Resources & Leaderboards](#resources--leaderboards)
- [Communities](#communities)

## Open-Weight Models

Models you can download and run on your own hardware. Most use permissive licenses (Apache 2.0, MIT, or custom open-weight licenses).

### Llama Family (Meta)

The industry standard for open-weight models. Optimized for local hardware with extensive quantization support.

- [Llama 4](https://huggingface.co/meta-llama) - Latest generation with Mixture-of-Experts architecture. Multiple sizes: Scout (109B, 1 active), Maverick (402B, 17 active). [[License]](https://github.com/facebookresearch/llama/blob/main/LICENSE)
- [Llama 3.3 70B](https://huggingface.co/meta-llama/Llama-3.3-70B-Instruct) - Top-tier instruct model, rivals GPT-4 on many benchmarks.
- [Llama 3.1 8B / 70B / 405B](https://huggingface.co/meta-llama) - Widely adopted, massive ecosystem of fine-tunes and tools.
- [Llama 3.2 1B / 3B / 11B / 90B](https://huggingface.co/meta-llama) - Includes small edge-friendly models (1B, 3B) and multimodal vision models (11B, 90B).

**License:** Custom open-weight license — permissive for most use cases, restrictions on large-scale commercial services (>700M MAU).

**Download:** [Hugging Face](https://huggingface.co/meta-llama) | GGUF quantized versions on [huggingface.co](https://huggingface.co/models?search=llama+gguf)

### Qwen Family (Alibaba)

Top-tier performers across language, code, and vision tasks. Released under Apache 2.0.

- [Qwen3 0.6B / 1.7B / 7B / 14B / 32B / 110B / 235B](https://huggingface.co/Qwen) - Latest generation. Excellent reasoning, multilingual support. Apache 2.0.
- [Qwen3-Coder](https://huggingface.co/Qwen/Qwen3-Coder-14B) - Code-specialized variant, state-of-the-art for open-weight coding.
- [Qwen3-VL](https://huggingface.co/Qwen/Qwen3-VL-7B) - Vision-language model, strong on document and image understanding.
- [Qwen2.5 7B / 32B / 72B](https://huggingface.co/Qwen) - Mature ecosystem, tons of community fine-tunes and tools.
- [Qwen2.5-Coder 1.5B / 7B / 32B](https://huggingface.co/Qwen) - Code-specialized, rivals GPT-4 on coding benchmarks.
- [Qwen2.5-VL 3B / 7B / 72B](https://huggingface.co/Qwen) - Vision-language model.

**License:** Apache 2.0 — fully permissive for commercial use.

### Mistral Family

Known for high-quality, efficient models that run well on consumer hardware.

- [Mistral Large](https://huggingface.co/mistralai) - Mistral's most capable open-weight model.
- [Mistral Small 3.1 24B](https://huggingface.co/mistralai) - High performance in a compact 24B package. Apache 2.0.
- [Mistral Small 3 24B](https://huggingface.co/mistralai) - Outperforms Llama 3.3 70B on several benchmarks at 1/3 the size.
- [Mistral 7B](https://huggingface.co/mistralai) - Classic 7B model, huge community ecosystem.
- [Mixtral 8x7B / 8x22B](https://huggingface.co/mistralai) - Mixture-of-Experts models offering high capability per compute.
- [Codestral](https://huggingface.co/mistralai) - Code-specialized models with permissive license.

**License:** Apache 2.0 (Small 3, Codestral), Mistral Research License, or Mistral Commercial License. Check each model's page.

### DeepSeek Family

Exceptional reasoning and coding performance. Known for efficiency innovations.

- [DeepSeek V3](https://huggingface.co/deepseek-ai/DeepSeek-V3) - Large MoE model rivaling top closed-source models.
- [DeepSeek R1](https://huggingface.co/deepseek-ai/DeepSeek-R1) - Reasoning-focused model with chain-of-thought capabilities.
- [DeepSeek Coder V2 / V3](https://huggingface.co/deepseek-ai) - State-of-the-art code generation and completion.
- [DeepSeek V2](https://huggingface.co/deepseek-ai) - Previous generation, still very capable.

**License:** MIT (most models) — fully permissive for commercial use.

### Gemma Family (Google)

Google's open-weight line. Excellent efficiency and quality.

- [Gemma 3 1B / 4B / 12B / 27B](https://huggingface.co/google) - Latest generation with strong multilingual and reasoning performance.
- [Gemma 2 2B / 9B / 27B](https://huggingface.co/google) - Widely adopted, punch above their weight class.
- [CodeGemma 2B / 7B](https://huggingface.co/google) - Code-specialized variants.
- [EmbeddingGemma 300M](https://huggingface.co/google) - Lightweight embedding model for RAG.

**License:** Custom open-weight license — generally permissive including commercial use.

### Phi Family (Microsoft)

Small models that punch far above their weight. Perfect for edge deployment and fast local inference.

- [Phi-4 14B](https://huggingface.co/microsoft/phi-4) - Microsoft's latest, rivals models 2-3x its size.
- [Phi-3 Mini (3.8B) / Small (7B) / Medium (14B)](https://huggingface.co/microsoft) - Run on phones and laptops.
- [Phi-3 Vision (4.2B)](https://huggingface.co/microsoft) - Small multimodal model.
- [Phi-3.5 MoE (4x3.8B)](https://huggingface.co/microsoft) - Mixture-of-Experts variant.

**License:** MIT (Phi-3 family), custom (Phi-4) — check each model.

### Other Notable Models

- [GLM-4 / GLM-4V (Zhipu AI)](https://huggingface.co/THUDM) - Strong multilingual model, MIT license.
- [Falcon 2 / 3 (TII)](https://huggingface.co/tiiuae) - Apache 2.0, available in multiple sizes.
- [Yi 1.5 / Yi 1.5-Chat (01.AI)](https://huggingface.co/01-ai) - Strong bilingual (Chinese/English) models.
- [Dbrx (Databricks)](https://huggingface.co/databricks) - MoE model, permissive license.
- [Kimi K2 (Moonshot AI)](https://huggingface.co/moonshotai) - Recent strong performer in reasoning tasks.
- [Solar Pro / Mini (Upstage)](https://huggingface.co/upstage) - Strong LLM with permissive license.
- [Command R / R+ (Cohere)](https://huggingface.co/CohereForAI) - Optimized for RAG, CC-BY-NC (free for non-commercial).
- [Hermes 3 (Nous Research)](https://huggingface.co/NousResearch) - Top-performing fine-tunes with strong instruction following. Apache 2.0.
- [OLMo 2 (AI2)](https://huggingface.co/allenai) - Fully open model — weights, training data, and code all released. Apache 2.0.
- [Nemotron / Nemo (NVIDIA)](https://huggingface.co/nvidia) - NVIDIA's open models, competitive with leading alternatives. permissive license.
- [Aya 23 / Aya Expanse (Cohere)](https://huggingface.co/CohereForAI) - Multilingual models covering 23+ languages. Apache 2.0.

## Free API Providers

Providers offering free tiers to access models via API — no local hardware required.

- [Google AI Studio](https://aistudio.google.com/) - **Most generous free tier.** Access Gemini 2.5 Flash, Gemini 2.0 Flash, and other models. Generous rate limits for prototyping. Data may be used for training unless configured otherwise.
- [OpenRouter](https://openrouter.ai/) - Aggregates 500+ models. Filter by "Free" to see models available at no cost. Includes experimental models, community models, and subsidized open-weight models.
- [Groq](https://console.groq.com/) - Ultra-fast inference. Free tier includes Llama, Gemma, Mixtral, Whisper models with generous daily rate limits.
- [Hugging Face Inference API](https://huggingface.co/inference-api) - Free tier for thousands of community models. Rate-limited but excellent for testing and light usage.
- [NVIDIA NIM](https://build.nvidia.com/) - Free API access to accelerated versions of Llama, Mistral, Gemma, and more on NVIDIA infrastructure.
- [DeepInfra](https://deepinfra.com/) - Serverless inference. Free tier with daily rate limits for popular open-source models.
- [Together AI](https://www.together.ai/) - Free trial credits for new users. Fast inference on open-source models.
- [Fireworks AI](https://fireworks.ai/) - Free tier for community models. Optimized for low latency.
- [Perplexity Labs](https://labs.perplexity.ai/) - Free access to Sonar models and open-source models for testing.
- [SiliconFlow](https://siliconflow.cn/) - Rising platform with free access to many open-source models.
- [Cloudflare Workers AI](https://developers.cloudflare.com/workers-ai/) - Free tier for running select open-source models at the edge.
- [Replicate](https://replicate.com/) - Free tier with limited credits for running open-source models.

## Local Inference Tools

Run models on your own machine — no API keys needed, full privacy.

- [Ollama](https://ollama.com/) - The easiest way to run local LLMs. One command to download and run any model. Supports GGUF, GPU acceleration. macOS, Linux, Windows. [GitHub](https://github.com/ollama/ollama)
- [LM Studio](https://lmstudio.ai/) - Polished desktop GUI. Browse, download, and chat with models. Built-in search, model management, and local API server. macOS, Linux, Windows.
- [llama.cpp](https://github.com/ggerganov/llama.cpp) - High-performance C++ inference engine. Runs on CPU and GPU. Supports quantization (GGUF format). Powers most other local tools.
- [Jan](https://jan.ai/) - Open-source ChatGPT alternative for desktop. Built-in model downloader, local API server. [GitHub](https://github.com/janhq/jan)
- [GPT4All](https://gpt4all.io/) - Privacy-focused local chatbot. Runs on consumer hardware. Built-in model browser. [GitHub](https://github.com/nomic-ai/gpt4all)
- [text-generation-webui (Oobabooga)](https://github.com/oobabooga/text-generation-webui) - Feature-rich web UI for running models. Supports multiple backends (Transformers, llama.cpp, ExLlama, AutoGPTQ). Gradio interface.
- [LocalAI](https://localai.io/) - Drop-in OpenAI API replacement. Run models locally with an OpenAI-compatible API. [GitHub](https://github.com/mudler/LocalAI)
- [KoboldCPP](https://github.com/LostRuins/koboldcpp) - Single-file executable for running GGUF models. Focused on story generation but general-purpose.
- [llamafile (Mozilla)](https://github.com/Mozilla-Ocho/llamafile) - Distributable single-file executables that run LLMs. No installation needed.
- [vLLM](https://github.com/vllm-project/vllm) - High-throughput production inference engine. Best for serving models with PagedAttention.
- [TensorRT-LLM (NVIDIA)](https://github.com/NVIDIA/TensorRT-LLM) - NVIDIA's optimized inference engine. Best performance on NVIDIA GPUs.
- [ExLlamaV2](https://github.com/turboderp/exllamav2) - Optimized inference for Llama-family models. Fastest option for single-GPU inference.
- [llama.cpp Server](https://github.com/ggerganov/llama.cpp/tree/master/examples/server) - Built-in HTTP server in llama.cpp, OpenAI-compatible API.

## Multimodal & Vision Models

Free models that understand images, video, and documents.

- [Qwen3-VL 7B / 72B](https://huggingface.co/Qwen) - State-of-the-art open vision-language model. Document understanding, image captioning, visual Q&A.
- [Qwen2.5-VL 3B / 7B / 72B](https://huggingface.co/Qwen) - Mature vision-language model with strong multilingual OCR.
- [Llama 3.2 Vision 11B / 90B](https://huggingface.co/meta-llama) - Meta's vision-language models integrated with Llama ecosystem.
- [Pixtral 12B (Mistral)](https://huggingface.co/mistralai) - Mistral's multimodal model with strong document understanding.
- [GLM-4V-9B (Zhipu AI)](https://huggingface.co/THUDM/glm-4v-9b) - Vision-language model, MIT license.
- [Florence-2 (Microsoft)](https://huggingface.co/microsoft/Florence-2-large) - Lightweight vision model for captioning, detection, segmentation.
- [SigLIP (Google)](https://huggingface.co/google/siglip-so-vit-patch16-256) - Vision encoder for multimodal applications.
- [PaliGemma (Google)](https://huggingface.co/google/paligemma) - Vision-language model built on Gemma.

## Code Models

Specialized for code generation, completion, and analysis.

- [Qwen3-Coder 14B](https://huggingface.co/Qwen/Qwen3-Coder-14B) - State-of-the-art open-weight code model. Apache 2.0.
- [Qwen2.5-Coder 1.5B / 7B / 32B](https://huggingface.co/Qwen) - Excellent multi-language code generation.
- [DeepSeek-Coder V2 / V3](https://huggingface.co/deepseek-ai) - Rivals GPT-4 on coding benchmarks. MIT license.
- [Codestral (Mistral)](https://huggingface.co/mistralai) - Mistral's code model with permissive license.
- [CodeGemma 2B / 7B (Google)](https://huggingface.co/google) - Lightweight code models for completion and generation.
- [Code Llama 7B / 13B / 34B / 70B (Meta)](https://huggingface.co/meta-llama) - Meta's code-specialized Llama variants.
- [StarCoder2 3B / 7B / 15B](https://huggingface.co/bigcode) - Trained on The Stack v2 (619 programming languages). Apache 2.0.
- [Stable Code 3B](https://huggingface.co/stabilityai) - Compact code model by Stability AI.

## Embedding Models

Free models for semantic search, RAG, and text similarity.

- [BGE-M3 (BAAI)](https://huggingface.co/BAAI/bge-m3) - Top-tier multilingual embedding. Supports dense and sparse retrieval. Apache 2.0.
- [BGE-Large / Small / Base (BAAI)](https://huggingface.co/BAAI) - Family of embedding models for different performance/speed tradeoffs. Apache 2.0.
- [E5-Mistral 7B (intfloat)](https://huggingface.co/intfloat/e5-mistral-7b-instruct) - LLM-based embedding with state-of-the-art performance. MIT.
- [E5-Small / Base / Large (intfloat)](https://huggingface.co/intfloat) - Efficient embedding models. MIT.
- [gte-large / gte-small (Alibaba)](https://huggingface.co/Alibaba-NLP) - Strong general-purpose embeddings. Apache 2.0.
- [EmbeddingGemma 300M (Google)](https://huggingface.co/google/embedding-gemma-300M) - Lightweight, fast embedding for Edge devices.
- [Qwen-Embedding 8B](https://huggingface.co/Qwen) - High-performance embedding for RAG pipelines.
- [jina-embeddings-v3 (Jina AI)](https://huggingface.co/jinaai/jina-embeddings-v3) - Multi-task embedding model. Apache 2.0.
- [Nomic Embed Text V1 (Nomic AI)](https://huggingface.co/nomic-ai/nomic-embed-text-v1.5) - Long-context embedding (8192 tokens). Apache 2.0.
- [Sentence Transformers (SBERT)](https://www.sbert.net/) - Library and model hub for computing sentence embeddings. Pre-trained models for 100+ languages.

## Image Generation Models

Free, open models for generating images.

- [Stable Diffusion 3.5 / 3 (Stability AI)](https://huggingface.co/stabilityai) - Latest SD generation, improved prompt adherence and typography.
- [Stable Diffusion XL (SDXL)](https://huggingface.co/stabilityai/stable-diffusion-xl-base-1.0) - Mature, widely adopted with thousands of fine-tunes and LoRAs.
- [FLUX.1 (Black Forest Labs)](https://huggingface.co/black-forest-labs) - State-of-the-art open image generation. Multiple variants: dev (non-commercial), schnell (Apache 2.0).
- [Playground v3 (Playground AI)](https://huggingface.co/playgroundai) - High-quality image generation with strong prompt understanding.
- [DeepFloyd IF (Stability AI)](https://huggingface.co/DeepFloyd) - Text-to-image model with exceptional text rendering.
- [LCM-LoRA (Latent Consistency Models)](https://huggingface.co/latent-consistency) - Real-time image generation in 1-4 steps.

**Where to run:** Locally via [ComfyUI](https://github.com/comfyanonymous/ComfyUI), [Automatic1111 WebUI](https://github.com/AUTOMATIC1111/stable-diffusion-webui), [InvokeAI](https://github.com/invoke-ai/InvokeAI), or for free on [Hugging Face Spaces](https://huggingface.co/spaces).

## Audio & Speech Models

- [Whisper (OpenAI)](https://github.com/openai/whisper) - State-of-the-art speech-to-text. Multiple sizes (tiny to large). MIT license.
- [Whisper.cpp](https://github.com/ggerganov/whisper.cpp) - High-performance port of Whisper. Runs on CPU.
- [Bark (Suno)](https://github.com/suno-ai/bark) - Text-to-audio generation (speech, music, sound effects). MIT.
- [Kokoro](https://huggingface.co/facebook/kokoro) - Fast, lightweight TTS model. 82MB, runs on CPU.
- [Coqui TTS](https://github.com/coqui-ai/TTS) - Deep learning for text-to-speech. 1100+ languages.
- [MusicGen (Meta)](https://github.com/facebookresearch/audiocraft) - Music generation from text descriptions. CC-BY-NC 4.0.
- [Stable Audio Open (Stability AI)](https://huggingface.co/stabilityai/stable-audio-open-1.0) - Generate audio from text prompts. Apache 2.0.

## Fine-tuning Tools

Tools to fine-tune free models on your own data — all free and open-source.

- [Unsloth](https://github.com/unslothai/unsloth) - Fast memory-efficient fine-tuning. 2x faster, 50% less memory. Supports QLoRA, LoRA, full fine-tune.
- [Axolotl](https://github.com/OpenAccess-AI-Collective/axolotl) - Streamlined fine-tuning framework with support for multiple model architectures and quantization methods.
- [LLaMA-Factory](https://github.com/hiyouga/LLaMA-Factory) - Easy-to-use fine-tuning with web UI. Supports 100+ models, multiple training methods.
- [Hugging Face TRL](https://github.com/huggingface/trl) - Transformer Reinforcement Learning library. SFT, PPO, DPOTrainer for aligning models.
- [TorchTune (Meta)](https://github.com/pytorch/torchtune) - Native PyTorch library for fine-tuning LLMs. Simple, extensible, and efficient.
- [AutoTrain (Hugging Face)](https://github.com/huggingface/autotrain-advanced) - No-code fine-tuning platform. Train models with a web UI or API.

## Model Hosting Platforms

Free platforms that host models — run inference without downloading anything.

- [Hugging Face Spaces](https://huggingface.co/spaces) - Free hosting for ML apps (Gradio, Streamlit). Thousands of community demos.
- [Hugging Face Inference Endpoints (Free Tier)](https://huggingface.co/inference-endpoints) - Deploy models with free trial credits.
- [Google Colab (Free Tier)](https://colab.research.google.com/) - Free GPU (T4, sometimes A100). Perfect for running models and fine-tuning.
- [Kaggle Notebooks](https://www.kaggle.com/code) - Free GPU (T4 x2). 30 hours/week. Good for heavier workloads.
- [Lightning AI Studio](https://lightning.ai/) - Free tier with GPU access for development and prototyping.
- [Modal](https://modal.com/) - Free monthly credits for serverless GPU compute.
- [Replicate (Free Tier)](https://replicate.com/) - Free credits for running community models.
- [Deepnote](https://deepnote.com/) - Free tier with GPU for data science and ML notebooks.

## Resources & Leaderboards

- [Hugging Face Open LLM Leaderboard](https://huggingface.co/spaces/open-llm-leaderboard/open_llm_leaderboard) - The primary benchmark for open-weight models. Updated regularly.
- [LMSYS Chatbot Arena](https://lmarena.ai/) - Human preference rankings of models. Best source for real-world quality comparisons.
- [Artificial Analysis](https://artificialanalysis.ai/) - Independent benchmarks for speed, pricing, and quality across providers.
- [Hugging Face Models](https://huggingface.co/models) - Search 1M+ models. Filter by license, task, framework.
- [OpenRouter Models](https://openrouter.ai/models) - Browse models available via API with pricing and free tiers.
- [Ollama Library](https://ollama.com/library) - Browse models available for one-command local setup.
- [cheahjs/free-llm-api-resources](https://github.com/cheahjs/free-llm-api-resources) - Community-maintained list of free LLM API resources.
- [SweetTea](https://www.sweettea.ai/) - Community voting on model quality and preference.

## Communities

- [Hugging Face Discord](https://discord.gg/huggingface) - Model releases, discussions, and community support.
- [r/LocalLLaMA](https://reddit.com/r/LocalLLaMA) - The largest Reddit community for running local LLMs.
- [Ollama Discord](https://discord.gg/ollama) - Ollama community for local model enthusiasts.
- [LM Studio Discord](https://discord.gg/lmstudio) - LM Studio community.
- [Hugging Face Forums](https://discuss.huggingface.co/) - Discussions on models, datasets, and Spaces.

## License

[![CC0](https://mirrors.creativecommons.org/presskit/buttons/88x31/svg/cc-zero.svg)](https://creativecommons.org/publicdomain/zero/1.0/)

To the extent possible under law, the author has waived all copyright and related or neighboring rights to this work.
