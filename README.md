# Awesome AIGC Image/Video Detection [![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

<p align="center">
    <img src="icon.png" alt="Overview" width="100%">
</p>

A curated collection of the latest research and resources on AI-Generated Image and Video Detection. This repository encompasses datasets, benchmarks, research papers, and practical detection tools.
 

🚀🚀🚀Contributions are welcome! If you find any missing papers, datasets, or tools, feel free to open an issue or submit a pull request.

## Contents
- [Hot Events](#-hot-events)
- [Benchmarks & Datasets](#benchmarks--datasets)
- [Research Papers](#research-papers)
  - [MLLM-Based](#mllm-based)
  - [Classification-Based](#classification-based)
- [Competitions](#competitions)
- [Practical Detection Tools](#practical-detection-tools)
- [About Our Team](#-about-our-team)

---

## 🔥 Hot Events
- [因为GPT-image-2，整个互联网都变成了巨大的黑暗森林](https://mp.weixin.qq.com/s/zua1k53RovAOk15Juy6q3g)
- [ChatGPT 图像 2.0 现已上线! 开启图像生成的新纪元](https://openai.com/zh-Hans-CN/index/introducing-chatgpt-images-2-0/)
- [谷歌Gemini生图的暗水印，被印度小哥破解了，成功率90%，Github揽星3k+](https://github.com/aloshdenny/reverse-SynthID)
- [炸裂！技术力究极恐怖！米哈游蔡浩宇首款AI生成视频大模型LPM1.0曝光！自定义虚拟角色？支持多语言+无限真实+无限时长，实现自由对话、唱歌、表演等效果](https://www.bilibili.com/video/BV12SQwBEEZd/?vd_source=dc916dd94382a611d2fc7ba992618065)

- [⭐️ 刚刚，阿里官方认领神秘「欢乐马」(HappyHorse)，来自ATH郑波团队](https://weibo.com/8214551477/5286126636237040)

- [就AI换脸合成、影视素材魔改等，中广联演员委员会发声明](https://m.thepaper.cn/newsDetail_forward_32880368)

- [Is the new video of Netanyahu AI-generated?](https://x.com/ripplexrpie/status/2033212021647270063?s=46)

- [Netanyahu, disappearing ring!](https://x.com/jacksonhinklle/status/2033543544124633345?s=46)

- [为什么内塔尼亚胡没能成功证明自己没死？](https://www.bilibili.com/video/BV1ygwXzVEns?buvid=ZF4153F466FA276C4159AA3E46125C0C024C&from_spmid=tm.recommend.0.0&is_story_h5=false&mid=enL%2FASv4UwiQw63hS3bfYw%3D%3D&plat_id=114&share_from=ugc&share_medium=iphone&share_plat=ios&share_session_id=83DD9880-F093-4A78-8337-FAE59EB0F9A0&share_source=COPY&share_tag=s_i&timestamp=1773807790&unique_k=FyMOQcn&up_id=346563107&vd_source=516db97bb15e7a9ee84b3097ee2ff160)

- [A photo of Iran’s bombed schoolgirl graveyard went viral. Why did AI say it wasn’t real?](https://www.theguardian.com/global-development/2026/mar/17/atrocity-ai-slop-verify-facts-iran-minab-graves)

- [How AI Content Detection is Being Weaponized in the Iran War](https://www.techpolicy.press/how-ai-content-detection-is-being-weaponized-in-the-iran-war/)

- [改变视频行业的AI，快来了(但有点恐怖) - Bilibili 影视飓风](https://www.bilibili.com/video/BV1A3cczZEf6/?spm_id_from=333.1387.homepage.video_card.click&vd_source=516db97bb15e7a9ee84b3097ee2ff160)

- [勘误致歉：今日发布的库里采访资讯为AI杜撰生成](https://m.hupu.com/bbs-share/637055192.html?share=share&euid=7vQPQEPpuWG8GWXVjyxIRtUcrudfXWKbBiuRjnUu2JY=&cid=160373438)

- [聊聊关于Seedance 2.0的风波 - 数字生命卡兹克](https://mp.weixin.qq.com/s/FzHUB8uSQllJviMu6SLMew)

- [Trump unveils his vision for 'Gaza Riviera' with AI video featuring belly dancers and luxury yachts](https://www.youtube.com/shorts/ZIwqq3RDuc0)

- [电商上演「魔法对轰」：卖家用AI假图骗下单，买家拿AI烂水果骗退款](https://36kr.com/p/3409700220685704)

---

## Benchmarks & Datasets

> **Modality Legend:** `[I]` Image | `[V]` Video | `[M]` Multi-modal

> **Annotation Type Legend:** 
> `Au`: Authenticity | `Ex`: Explainability | `Lo`: Localization

| Benchmark | Paper | Venue & Year | Modality | Notes | Real Source | Fake Source/Generator | Annotation | Scale | Download |
| :-------- | :---- | :----------- | :------- | :------ | :---------- | :-------------------- | :--------- | :---- | :------- |
| SciFigDetect | [SciFigDetect: A Benchmark for AI-Generated Scientific Figure Detection](https://arxiv.org/pdf/2604.08211) | Arxiv 2026 | `[I]` | Scientific Figure Detection | | Nano Banana Pro, GPT-image-1.5 | `Au` | 150K | [SciFigDetect](https://joyce-yoyo.github.io/SciFigDetect/#access) |
| ActivityForensics | [ActivityForensics: A Comprehensive Benchmark for Localizing Manipulated Activity in Videos](https://arxiv.org/pdf/2604.03819) | CVPR 2026 | `[V]` | Action-level AIGC in videos | | | `Au` | 6K | [ActivityForensics](https://activityforensics.github.io/) |
| MintVid | [VideoVeritas: AI-Generated Video Detection via Perception Pretext Reinforcement Learning](https://arxiv.org/pdf/2602.08828) | Arxiv 2026 | `[V]` | | OpenVid, VFHQ, HDTF, TikTok | Jimeng3.0-Pro, Seedance, Kling2.5-Turbo, Sora2, TikTok, Youtube, etc.  | `Au` | 4K | [MintVid](https://www.modelscope.cn/datasets/EricTanh/MintVid) |
| AIGVDBench | [Your One-Stop Solution for AI-Generated Video Detection](https://arxiv.org/pdf/2601.11035) | CVPR 2026 | `[V]` | | OpenVid-HD | 31 generation models | `Au` | 440k | [AIGVDBench](https://huggingface.co/datasets/AIGVDBench/AIGVDBench) |
| HydraFake | [Veritas: Generalizable Deepfake Detection via Pattern-Aware Reasoning](https://arxiv.org/pdf/2508.21048) | ICLR 2026(Oral) | `[I]` | | FFHQ, VFHQ, CelebAHQ, FF++, etc. | GPT-4o, HailuoAI, ICLight, InfiniteYou, etc. | `Au`, `Ex` | 100K | [HydraFake](https://www.modelscope.cn/datasets/EricTanh/HydraFake) |
| BR-Gen | [Zooming In on Fakes: A Novel Dataset for Localized AI-Generated Image Detection with Forgery Amplification Approach](https://arxiv.org/abs/2504.11922) | AAAI 2026 | `[I]` | |  |  | `Au`, `Lo` | 150K | [BR-Gen](https://github.com/clpbc/BR-Gen) |
| HiResolution | [No Pixel Left Behind: A Detail-Preserving Architecture for Robust High-Resolution AI-Generated Image Detection](https://arxiv.org/pdf/2508.17346) | ICLR 2026 | `[I]` | |  |  | `Au` | 50K | [HiRes-50K](https://huggingface.co/datasets/Mu437/HiRes-50K) |
| AIGI-Now | [AlignGemini: Generalizable AI-Generated Image Detection Through Task-Model Alignment](https://arxiv.org/abs/2512.06746) | Arxiv 2026 | `[I]` | | COCO | Nano Banana, GPT-4o, Jimeng, Kling, Minimax, etc. | `Au` | 18K | [AIGI-Now](https://huggingface.co/datasets/Gaffeyzz/AIGI-Now) |
| RealChain | [Beyond Artifacts: Real-Centric Envelope Modeling for Reliable AI-Generated Image Detection](https://arxiv.org/pdf/2512.20937) | Arxiv 2026 | `[I]` | |  |  | `Au` | 14K | [RealChain](https://github.com/handsome-rich/REM) |
| GenVidBench | [GenVidBench: A 6-Million Benchmark for AI-Generated Video Detection](https://arxiv.org/pdf/2501.11340) | AAAI 2026 | `[V]` | |  |  | `Au` | 6M | [GenVidBench](https://huggingface.co/datasets/jian-0/GenVidBench/tree/main) |
| Skyra | [Skyra: AI-Generated Video Detection via Grounded Artifact Reasoning](https://arxiv.org/pdf/2512.15693) | CVPR 2026 | `[V]` | |  |  | `Au`, `Ex`, `Lo` | 4K | [ViF-CoT-4K](https://huggingface.co/datasets/JoeLeelyf/ViF-CoT-4K) |
| So-Fake-Set | [So-Fake: Benchmarking and Explaining Social Media Image Forgery Detection](https://arxiv.org/pdf/2505.18660) | Arxiv 2025 | `[I]` | | F30k, WIDER, FFHQ, CelebA, OpenImages, COCO, OpenForensics | Qwen-image, GPT-4o, Nano Banana, Seedream3.0, Ideogram3.0, etc. | `Au` | 2M+ | [So-Fake-Set](https://huggingface.co/datasets/saberzl/So-Fake-Set) <br> [So-Fake-OOD](https://huggingface.co/datasets/saberzl/So-Fake-OOD)|
| GenBuster++ | [BusterX++: Towards Unified Cross-Modal AI-Generated Content Detection and Explanation with MLLM](https://arxiv.org/pdf/2507.14632) | Arxiv 2025 | `[M]` | |  |  | `Au` | 4K | [GenBuster++](https://huggingface.co/datasets/l8cv/GenBuster_plusplus) | 
| GenBuster | [BusterX: MLLM-Powered AI-Generated Video Forgery Detection and Explanation](https://arxiv.org/pdf/2505.12620) | Arxiv 2025 | `[I]` | |  |  | `Au` | 200K | [GenBuster-200K](https://huggingface.co/datasets/l8cv/GenBuster-200K) |
| AIGIBench| [Is Artificial Intelligence Generated Image Detection a Solved Problem?](https://arxiv.org/pdf/2505.12335) | NeurIPS 2025 | `[I]` | | FFHQ, CelebA-HQ, Open Images V7 | Common generators & SocialRF, CommunityAI | `Au` | 200K | [AIGIBench](https://huggingface.co/datasets/HorizonTEL/AIGIBench) |
| Ivy-Fake | [IVY-FAKE: A Unified Explainable Framework and Benchmark for Image and Video AIGC Detection](https://arxiv.org/pdf/2506.00979) | Arxiv 2025 | `[M]` | |  |  | `Au`, `Ex` | 150K | [Ivy-Fake](https://huggingface.co/datasets/AI-Safeguard/Ivy-Fake) |
| AEGIS | [AEGIS: Authenticity Evaluation Benchmark for AI-Generated Video Sequences](https://dl.acm.org/doi/10.1145/3746027.3758295) | ACM MM 2025 | `[V]` | | Vript (YouTube, TikTok), DVF, YouTube (self-collected) | Stable Video Diffusion, CogVideoX-5B, I2VGen-XL, Pika, KLing, Sora | `Au`, `Ex` | 10K+ | [AEGIS](https://huggingface.co/datasets/Clarifiedfish/AEGIS) |
| NeXT-IMDL | [NeXT-IMDL: Build Benchmark for Next-Generation Image Manipulation Detection & Localization](https://arxiv.org/abs/2512.23374) | Arxiv 2025 | `[I]` | | Flickr30k, COCO, OpenImages V7 | SD2-Inpainting, SDXL-Inpainting, FLUX-Inpainting, etc. | `Au`, `Lo` | 558K | [NeXT-IMDL](https://github.com/JoeLeelyf/NeXT-IMDL) |
| ARForensics | [D3QE: Learning Discrete Distribution Discrepancy-aware Quantization Error for Autoregressive-Generated Image Detection](https://openaccess.thecvf.com/content/ICCV2025/papers/Zhang_D3QE_Learning_Discrete_Distribution_Discrepancy-aware_Quantization_Error_for_Autoregressive-Generated_Image_ICCV_2025_paper.pdf) | ICCV 2025 | `[I]` | | ImageNet | Infinity, Janus_Pro, RAR, Switti, VAR, LlamaGen, Open_MAGVIT2 | `Au` | 300k | [ARForensics](https://huggingface.co/datasets/Yanran21/ARForensics) |
| OpenSDI | [OpenSDI: Spotting Diffusion-Generated Images in the Open World](https://openaccess.thecvf.com/content/CVPR2025/papers/Wang_OpenSDI_Spotting_Diffusion-Generated_Images_in_the_Open_World_CVPR_2025_paper.pdf) | CVPR 2025 | `[I]` | | Megalith-10M | SD1.5, SD2.1, SDXL, SD3, Flux.1 | `Au`, `Lo` | 300K | [OpenSDI](https://github.com/iamwangyabin/OpenSDI) |
| Community Forensics | [Community Forensics: Using Thousands of Generators to Train Fake Image Detectors](https://openaccess.thecvf.com/content/CVPR2025/papers/Park_Community_Forensics_Using_Thousands_of_Generators_to_Train_Fake_Image_Detectors_CVPR_2025_paper.pdf) | CVPR 2025 | `[I]` | | LAION, ImageNet, COCO, FFHQ, CelebA, MetFaces, AFHQ, etc. | 4803 generators (Latent Diffusion, GAN, Autoregressive, Pixel Diffusion, Commercial) | `Au` | 2.7M | [Community Forensics](https://jespark.net/projects/2024/community_forensics) |
| FakeClue | [Spot the Fake: Large Multimodal Model-Based Synthetic Image Detection with Artifact Explanation](https://arxiv.org/pdf/2503.14905) | NeurIPS 2025 | `[I]` | |  |  | `Au`, `Ex` | 100K | [FakeClue](https://huggingface.co/datasets/lingcco/FakeClue) |
| XAIGID-RewardBench | [Explainable AI-Generated Image Detection RewardBench](https://arxiv.org/abs/2511.12363) | NeurIPS 2025 Workshop | `[I]` | | COCO-2017 | Imagen 4, Flux.1 Dev, Bagel, etc. | `Au`, `Ex` | 3K | [XAIGID-RewardBench](https://github.com/RewardBench/XAIGID-RewardBench) |
| RewardData | [Learning Human-Perceived Fakeness in AI-Generated Videos via Multimodal LLMs](https://arxiv.org/pdf/2509.22646) | Arxiv 2025 | `[V]` | |  |  | `Au`, `Ex` | 4.3K | [RewardData](https://huggingface.co/datasets/DeeptraceReward/RewardData) |
| OpenFake | [OPENFAKE: An Open Dataset and Platform Toward Real-World Deepfake Detection](https://arxiv.org/abs/2509.09495) | Arxiv 2025 | `[I]` | | LAION-400M | SD 1.5/2.1/XL/3.5, Flux 1.0-dev/1.1-Pro/Schnell, Midjourney v6/v7, DALL·E 3, Imagen 3/4, GPT Image 1, Ideogram 3.0, Grok-2, HiDream-I1, Recraft v3, Chroma, and 10 community LoRA/finetune variants | `Au` | ~4M | [OPENFAKE](https://huggingface.co/datasets/ComplexDataLab/OpenFake) |
| Video Reality Test | [Video Reality Test: Can AI-Generated ASMR Videos fool VLMs and Humans?](https://arxiv.org/abs/2512.13281) | Arxiv 2025 | `[V]` | | YouTube ASMR (social media) | Veo3.1-Fast, Sora2, Wan2.2-A14B, Wan2.2-5B, OpenSora-V2, HunyuanVideo, StepVideo | `Au` | 149 real + dynamic fake | [Video Reality Test](https://video-reality-test.github.io/) |
| DDL | [DDL: A Dataset for Interpretable Deepfake Detection and Localization in Real-World Scenarios](https://arxiv.org/pdf/2506.23292v1) | Arxiv 2025 | `[M]` | |  |  | `Au` | 367K | [DDL](https://deepfake-workshop-ijcai2025.github.io/main/index.html) |
| DiffSeg30k | [DiffSeg30k: A Multi-Turn Diffusion Editing Benchmark for Localized AIGC Detection](https://arxiv.org/abs/2511.19111) | Arxiv 2025 | `[I]` | | COCO | SD2, SD3.5, SDXL, Flux.1, Glide, Kolors, HunyuanDiT1.1, Kandinsky 2.2 | `Au`, `Lo` | 30K | [DiffSeg30k](https://huggingface.co/datasets/Chaos2629/Diffseg30k) |
| FakeParts | [FakeParts: a New Family of AI-Generated DeepFakes](https://arxiv.org/abs/2508.21052) | Arxiv 2025 | `[V]` | | | | `Au`, `Lo` | 81K | [FakeParts](https://huggingface.co/datasets/hi-paris/FakeParts) |
| ForensicHub | [ForensicHub: A Unified Benchmark & Codebase for All-Domain Fake Image Detection and Localization](https://arxiv.org/abs/2505.11003) | NeurIPS 2025 | `[I]` | |  | ProGAN, StyleGAN, LDM, SDv1.4, SDv1.5, SDv2, SDXL, SD-ControlNet, MidJourney, ADM, GLIDE, VQDM, BigGAN | `Au`, `Lo` | 23 datasets <br> 42 models | [ForensicHub](https://github.com/scu-zjz/ForensicHub) |
| LOKI | [LOKI: A Comprehensive Synthetic Data Detection Benchmark Using Large Multimodal Models](https://arxiv.org/abs/2410.09732) | ICLR 2025 | `[M]` | |  | SORA, Keling, Open-Sora, FLUX, Midjourney, Stable Diffusion, Nerf-based, Gaussian-based, GPT-4o, Qwen-Max, Llama 3.1-405B, MusicGen, AudioLDM2... | `Au`, `Ex` | 18K | [LOKI](https://opendatalab.github.io/LOKI/) |
| Chameleon | [A Sanity Check for AI-Generated Image Detection](https://arxiv.org/abs/2406.19435) | ICLR 2025 | `[I]` | | Unsplash | Midjourney, DALLE-3, Stable Diffusion (various LoRA fine-tuned) | `Au` | 26K | [Chameleon](https://shilinyan99.github.io/AIDE/index_aide.html) |
| WildFake| [WildFake: A Large-scale Challenging Dataset for AI-Generated Images Detection](https://arxiv.org/pdf/2402.11843) | AAAI 2025 | `[I]` | |  |  | `Au` | 3.7M | [WildFake](https://modelscope.cn/datasets/hy2628982280/WildFake/summary) |
| WildRF | [Real-Time Deepfake Detection in the Real-World](https://arxiv.org/abs/2406.09398) | Arxiv 2024 | `[I]` | | Reddit, X (Twitter), Facebook (real images) | Reddit, X (Twitter), Facebook (social media deepfakes) | `Au` | | [WidlRF](https://vision.huji.ac.il/ladeda/) |
| AIGCDetectBenchmark | [PatchCraft: Exploring Texture Patch for Efficient AI-generated Image Detection](https://arxiv.org/pdf/2311.12397) | Arxiv 2024 | `[I]` | |  |  | `Au` | 100K | [AIGCDetectionBenchMark](https://modelscope.cn/datasets/aemilia/AIGCDetectionBenchmark/files) |
| GenVideo| [DeMamba: AI-Generated Video Detection on Million-Scale GenVideo Benchmark](https://arxiv.org/pdf/2405.19707) | Arxiv 2024 | `[V]` | |  |  | `Au` | 2.3M | [GenVideo](https://modelscope.cn/datasets/cccnju/Gen-Video) |
| DRCT | [Drct: Diffusion reconstruction contrastive training towards universal detection of diffusion generated images](https://openreview.net/pdf?id=oRLwyayrh1) | ICML 2024 | `[I]` | | MSCOCO | LDM, SDv1.4, SDv1.5, SDv2, SDXL, SD-ControlNet | `Au` | 2M | [DRCT-2M](https://modelscope.cn/datasets/BokingChen/DRCT-2M/files) |
| GenImage| [GenImage: A Million-Scale Benchmark for Detecting AI-Generated Image](https://proceedings.neurips.cc/paper_files/paper/2023/file/f4d4a021f9051a6c18183b059117e8b5-Paper-Datasets_and_Benchmarks.pdf) | NeurIPS 2023 | `[I]` | | ImageNet, Wukong | MidJourney, SDv1.4, SDv1.5, ADM, GLIDE, VQDM, BigGAN | `Au` | 2.7M | [GenImage](https://drive.google.com/drive/folders/1jGt10bwTbhEZuGXLyvrCuxOI0cBqQ1FS) |
| DF40 | [DF40: Toward Next-Generation Deepfake Detection](https://arxiv.org/abs/2406.13495) | NeurIPS 2024 | `[I]` `[V]` | | | | `Au` | 0.1M+ videos, 1M+ images | [DF40](https://github.com/YZY-stack/DF40) |
| Forensics-Bench | [Forensics-Bench: A Comprehensive Forgery Detection Benchmark Suite for Large Vision Language Models](https://openaccess.thecvf.com/content/CVPR2025/papers/Wang_Forensics-Bench_A_Comprehensive_Forgery_Detection_Benchmark_Suite_for_Large_Vision_Language_Models_CVPR_2025_paper.pdf) | CVPR 2025 | `[I]`, `[V]`, `[M]` | | Various public datasets | GAN, Diffusion, VAE, RNN, Encoder-Decoder, Graphics-based | `Au`, `Lo` | 63K | [Forensics-Bench](https://forensics-bench.github.io/) |



⬆ [Back to Top](#contents)

---

## Research Papers

> **💡 Note:** Papers are sorted by year (descending) within each category. <br>
> **Modality Legend:** `[I]` Image | `[V]` Video | `[M]` Multi-modal

### MLLM-Based
*This category focuses on utilizing Multimodal Large Language Models (MLLMs) like GPT-4V, LLaVA, or Qwen-VL to detect AI-generated content. These methods often provide natural language explanations (explainability) alongside binary detection.*

| Title | Venue & Year | Modality | Highlights/Keywords | Code |
| --- | --- | --- | --- | --- |
| [VideoVeritas: AI-Generated Video Detection via Perception Pretext Reinforcement Learning](https://arxiv.org/pdf/2602.08828) | Arxiv 2026 | `[V]` | Perception Pretext RL, Fact-based Reasoning, MintVid Dataset | [GitHub](https://github.com/EricTan7/VideoVeritas) |
| [Veritas: Generalizable deepfake detection via pattern-aware reasoning](https://arxiv.org/pdf/2508.21048) | ICLR 2026(Oral) | `[I]` | Pattern-aware Reasoning, HydraFake Dataset | [Github](https://github.com/EricTan7/Veritas) |
| [DF-LLaVA: Unlocking MLLMs for Synthetic Image Detection via Knowledge Injection and Conflict-Driven Self-Reflection](https://arxiv.org/pdf/2509.14957) | Arxiv 2026 | `[I]` | Knowledge Injection, Self-Reflection | N/A |
| [DocShield: Towards AI Document Safety via Evidence-Grounded Agentic Reasoning](https://arxiv.org/pdf/2604.02694) | Arxiv 2026 | `[M]` | Agentic Framework, Document Safety | N/A |
| [VidGuard-R1: AI-Generated Video Detection and Explanation via Reasoning MLLMs and RL](https://arxiv.org/abs/2510.02282) | ICLR 2026 | `[V]` | Multi-stage RL, Video Detection Dataset | [GitHub](https://github.com/kyoungjunpark/VidGuard-R1) |
| [FakeXplain: AI-Generated Image Detection via Human-Aligned Grounded Reasoning](https://arxiv.org/pdf/2506.07045) | ICLR 2026 | `[I]` | Grounded Reasoning, Human-annotated Dataset | N/A |
| [AlignGemini: Generalizable AI-Generated Image Detection Through Task-Model Alignment](https://arxiv.org/pdf/2512.06746) | Arxiv 2026 | `[I]` | Decoupling (Semantic & Pixel), AIGI-Now Dataset | N/A |
| [Zoom-In to Sort AI-Generated Images Out](https://arxiv.org/pdf/2510.04225) | ICLR 2026 | `[I]` | Thinking with Images, MagniFake Dataset | N/A |
| [AgentFoX: LLM Agent-Guided Fusion with eXplainability for AI-Generated Image Detection](https://arxiv.org/pdf/2603.23115) | Arxiv 2026 | `[I]` | Agentic framework | [Github](https://github.com/suncore946/AgentFoX) |
| [EvoGuard: An Extensible Agentic RL-based Framework for Practical and Evolving AI-Generated Image Detection](https://arxiv.org/pdf/2603.17343) | Arxiv 2026 | `[I]` | Agentic Framework, Method Ensembling | N/A |
| [VIGIL: Part-Grounded Structured Reasoning for Generalizable Deepfake Detection](https://arxiv.org/pdf/2603.21526) | Arxiv 2026 | `[I]` | Part-centric Forensic, OmniFake Dataset | [Project](https://vigil.best/) |
| [GenVideoLens: Where LVLMs Fall Short in AI-Generated Video Detection?](https://arxiv.org/pdf/2603.18625) | Arxiv 2026 | `[V]` | GenVideoLens benchmark | N/A |
| [Semantic Visual Anomaly Detection and Reasoning in AI-Generated Images](https://arxiv.org/pdf/2510.10231) | ICLR 2026 | `[I]` | Semantic Anomaly Reasoning, AnomReason Dataset | N/A |
| [FAKE-HR1: RETHINKING REASONING OF VISION LANGUAGE MODEL FOR SYNTHETIC IMAGE DETECTION](https://arxiv.org/pdf/2602.10042v1) | Arxiv 2026 | `[I]` | Hybrid-Reasoning, Dual-mode Dataset | N/A |
| [MIRAGE: Towards AI-Generated Image Detection in the Wild](https://arxiv.org/pdf/2508.13223) | Arxiv 2025 | `[I]` | Human Curation Dataset, Heuristic-to-Analytic Reasoning | N/A |
| [BusterX++: Towards Unified Cross-Modal AI-Generated Content Detection and Explanation with MLLM](https://www.alphaxiv.org/pdf/2507.14632) | Arxiv 2025 | `[M]` | RL Post-training, Cross-Modal, Thinking Reward Mechanism | [Github](https://github.com/l8cv/BusterX) |
| [BusterX: MLLM-Powered AI-Generated Video Forgery Detection and Explanation](https://www.alphaxiv.org/pdf/2505.12620) | Arxiv 2025 | `[V]` | GenBuster-200K Dataset, Cold Start + RL Training | [Github](https://github.com/l8cv/BusterX) |
| [REVEAL: Reasoning-enhanced Forensic Evidence Analysis for Explainable AI-generated Image Detection](https://arxiv.org/pdf/2511.23158) | Arxiv 2025 | `[I]` | Chain-of-Evidence, Expert-grounded RL | N/A |
| [Spot the Fake: Large Multimodal Model-Based Synthetic Image Detection with Artifact Explanation](https://arxiv.org/pdf/2503.14905) | NeurIPS 2025 | `[I]` | FakeClue Dataset, Fine-grained Artifact Clues, Artifact Explanation | [GitHub](https://github.com/opendatalab/FakeVLM) |
| [AIGI-Holmes: Towards Explainable and Generalizable AI-Generated Image Detection via Multimodal Large Language Models](https://arxiv.org/pdf/2507.02664) | ICCV 2025 | `[I]` | Holmes-Set, Multi-Expert Jury, 3-Stage Training Pipeline | [Github](https://github.com/wyczzy/AIGI-Holmes) |
| [LEGION: Learning to Ground and Explain for Synthetic Image Detection](https://arxiv.org/pdf/2503.15264) | ICCV 2025 | `[I]` | SynthScars Dataset, Defender & Controller, Image Refinement | [GitHub](https://github.com/opendatalab/LEGION) |
| [Seeing Before Reasoning: A Unified Framework for Generalizable and Explainable Fake Image Detection](https://arxiv.org/pdf/2509.25502) | Arxiv 2025 | `[I]` | Perception & Reasoning, ExplainFake-Bench | N/A |
| [SIDA: Social Media Image Deepfake Detection, Localization, and Explanation](https://arxiv.org/pdf/2412.04292) | CVPR 2025 | `[I]` | SID-Set, Mask Prediction, Social Media Context | [Github](https://github.com/hzlsaber/SIDA) |
| [FakeShield: Explainable Image Forgery Detection and Localization via Multi-modal Large Language Models](https://arxiv.org/pdf/2410.02761) | ICLR 2025 | `[I]` | Explainable IFDL, Domain Tag-guided, Multi-modal Localization | [GitHub](https://github.com/zhipeixu/FakeShield) |
| [VidGuard-R1: AI-Generated Video Detection and Explanation via Reasoning MLLMs and RL](https://arxiv.org/pdf/2510.02282) | ICLR 2026 | `[V]` | GRPO, Time Artifacts, Quality Evolutionary Videos | N/A |
| [FakeScope: Large Multimodal Expert Model for Transparent AI-Generated Image Forensics](https://arxiv.org/pdf/2503.24267) | Arxiv 2025 | `[I]` | FakeChain Dataset, FakeInstruct, Trace Evidence | N/A |
| [AntifakePrompt: Prompt-Tuned Vision-Language Models are Fake Image Detectors](https://arxiv.org/pdf/2310.17419) | Arxiv 2024 | `[I]` | VQA, InstructBLIP, Soft Prompt-tuning, Zero-shot | [GitHub](https://github.com/nctu-eva-lab/AntifakePrompt) |


### Classification-Based
*This category includes supervised learning approaches that train neural networks (CNNs, ViTs, etc.) specifically to classify authentic vs. AI-generated content. They usually focus on robustness, generalization, and feature extraction.*

| Title | Venue & Year | Modality | Highlights/Keywords | Code |
| --- | --- | --- | --- | --- |
| [Zooming In on Fakes: A Novel Dataset for Localized AI-Generated Image Detection with Forgery Amplification Approach](https://arxiv.org/abs/2504.11922) | AAAI 2026 | `[I]` | Localized AIGC Detection, Forgery Amplification, Scene-aware Local Forgery | [GitHub](https://github.com/clpbc/BR-Gen) |
| [Preserving Forgery Artifacts: AI-Generated Video Detection at Native Scale](https://openreview.net/pdf?id=XD43lfRCg6) | ICLR 2026 | `[V]` | Native scale video processing, Massive realistic video dataset, Preserves subtle generation artifacts | N/A |
| [Generalizable and Adaptive Continual Learning Framework for AI-generated Image Detection](https://arxiv.org/pdf/2601.05580) | TMM 2026 | `[I]` | Continual Learning, Kronecker-Factored Approximate Curvature | N/A |
| [Simplicity Prevails: The Emergence of Generalizable AIGI Detection in Visual Foundation Models](https://arxiv.org/pdf/2602.01738) | Arxiv 2026 | `[I]` | Linear Probe, Vision Foundation Models, Emergent Forensic Capability | N/A |
| [MIRROR: Manifold Ideal Reference ReconstructOR for Generalizable AI-Generated Image Detection](https://arxiv.org/pdf/2602.02222) | Arxiv 2026 | `[I]` | Manifold Reconstruction, Memory Bank, Human-AIGI Benchmark | [GitHub](https://github.com/349793927/MIRROR) |
| [No Pixel Left Behind: A Detail-Preserving Architecture for Robust High-Resolution AI-Generated Image Detection](https://arxiv.org/pdf/2508.17346) | ICLR 2026 | `[I]` | Detail-preserving dual-path architecture, Multi-task learning, HiRes-50K benchmark  | N/A |
| [All Patches Matter, More Patches Better: Enhance AI-Generated Image Detection via Panoptic Patch Learning](https://arxiv.org/pdf/2504.01396) | ICLR 2026 | `[I]` | Random Patch Replacement, Patch-wise Contrastive Learning  | N/A |
| [OmniAID: Decoupling Semantic and Artifacts for Universal AI-Generated Image Detection in the Wild](https://arxiv.org/pdf/2511.08423) | Arxiv 2025 | `[I]` | Mixture-of-Experts, Semantic-Artifact Decoupling, Mirage Dataset | [GitHub](https://github.com/yunncheng/OmniAID) |
| [DINO-Detect: A Simple yet Effective Framework for Blur-Robust AI-Generated Image Detection](https://arxiv.org/pdf/2511.12511) | Arxiv 2025 | `[I]` | Blur Robustness, Knowledge Distillation, DINOv3 | [Github](https://github.com/JiaLiangShen/Dino-Detect-for-blur-robust-AIGC-Detection) |
| [D3QE: Learning Discrete Distribution Discrepancy-aware Quantization Error for Autoregressive-Generated Image Detection](https://openaccess.thecvf.com/content/ICCV2025/papers/Zhang_D3QE_Learning_Discrete_Distribution_Discrepancy-aware_Quantization_Error_for_Autoregressive-Generated_Image_ICCV_2025_paper.pdf) | ICCV 2025 | `[I]` | Discrete Distribution Discrepancy-aware Transformer, Vector Quantized Variational AutoEncoder | [Github](https://github.com/Zhangyr2022/D3QE) |
| [Seeing What Matters: Generalizable AI-generated Video Detection with Forensic-Oriented Augmentation](https://arxiv.org/pdf/2506.16802) | NeurIPS 2025 | `[V]` | Wavelet-band Augmentation, Forensic Frequency Artifacts, Single-generator Generalization | [GitHub](https://github.com/grip-unina/WaveRep-SyntheticVideoDetection) |
| [AI-Generated Video Detection via Perceptual Straightening](https://arxiv.org/pdf/2507.00583) | NeurIPS 2025 | `[V]` | Perceptual Straightening, DINOv2, Temporal Curvature | [GitHub](https://github.com/ChristianInterno/ReStraV) |
| [Physics-Driven Spatiotemporal Modeling for AI-Generated Video Detection](https://arxiv.org/pdf/2510.08073) | NeurIPS 2025 | `[V]` | Normalized Spatiotemporal Gradient (NSG), Maximum Mean Discrepancy (MMD) | [Github](https://github.com/ZSHsh98/NSG-VD) |
| [Dual Data Alignment Makes AI-Generated Image Detector Easier Generalizable](https://arxiv.org/pdf/2505.14359) | NeurIPS 202 (Spotlight) | `[I]` | Dual-domain Alignment, Frequency-level Bias, VAE Reconstruction | [GitHub](https://github.com/roy-ch/Dual-Data-Alignment) |
| [Orthogonal Subspace Decomposition for Generalizable AI-Generated Image Detection](https://arxiv.org/pdf/2411.15633) | ICML 2025 (Oral) | `[I]` | SVD Orthogonal Subspace, Asymmetry Phenomenon, Parameter-efficient Fine-tuning | [GitHub](https://github.com/zhiyuan-yan/Effort) |
| [Any-Resolution AI-Generated Image Detection by Spectral Learning](https://arxiv.org/pdf/2411.19417) | CVPR 2025 | `[I]` | Spectral Context Attention, Frequency Reconstruction, OOD Detection | [Github](https://github.com/kartyg23/spai) |
| [A Bias-Free Training Paradigm for More General AI-generated Image Detection](https://arxiv.org/pdf/2412.17671) | CVPR 2025 | `[I]` | Bias-Free, Semantic Alignment, Stable Diffusion Self-conditioning | [Github](https://github.com/grip-unina/B-Free) |
| [Forensics Adapter: Adapting CLIP for Generalizable Face Forgery Detection](https://arxiv.org/pdf/2411.19715) | CVPR 2025 | `[I]` | CLIP, Blending Boundaries, Forgery-aware Prompt Learning | [Github](https://github.com/OUC-VAS/ForensicsAdapter) |
| [Towards a Universal Synthetic Video Detector: From Face or Background Manipulations to Fully AI-Generated Content](https://arxiv.org/pdf/2412.12278) | CVPR 2025 | `[V]` | SigLIP-So400M, Attention-Diversity Loss, Full-frame Manipulations | N/A |
| [Exploring Unbiased Deepfake Detection via Token-Level Shuffling and Mixing](https://arxiv.org/pdf/2501.04376) | AAAI 2025 | `[I]` | Token-Level Shuffling, Contrastive Loss, Bias Mitigation | N/A |
| [DIP: Diffusion Learning of Inconsistency Pattern for General DeepFake Detection](https://arxiv.org/pdf/2410.23663) | TMM 2025 | `[V]` | Direction-aware Attention, SpatioTemporal Invariant Loss | N/A |
| [Frequency-Aware Deepfake Detection: Improving Generalizability through Frequency Space Domain Learning](https://arxiv.org/pdf/2403.07240) | AAAI 2024 | `[I]` | Frequency Domain, FFT, Frequency Conv Layer (FCL), Lightweight | [GitHub](https://github.com/chuangchuangtan/FreqNet-DeepfakeDetection) |
| [DeMamba: AI-Generated Video Detection on Million-Scale GenVideo Benchmark](https://arxiv.org/pdf/2405.19707) | Arxiv 2024 | `[V]` | Mamba, State Space Model, Long-range Spatiotemporal Inconsistency | [GitHub](https://github.com/chenhaoxing/DeMamba) |
| [Rethinking the Up-Sampling Operations in CNN-based Generative Network](https://arxiv.org/pdf/2312.10461) | CVPR 2024 | `[I]` | Neighboring Pixel Relationships, Generalized Structural Artifacts | [Github](https://github.com/chuangchuangtan/NPR-DeepfakeDetection) |
| [Distinguish Any Fake Videos: Unleashing the Power of Large-scale Data and Motion Features](https://arxiv.org/pdf/2405.15343) | Arxiv 2024 | `[V]` | GenVidDet, Optical Flow, Dual-Branch 3D Transformer | N/A |
| [FakeFormer: Efficient Vulnerability-Driven Transformers for Generalisable Deepfake Detection](https://arxiv.org/pdf/2410.21964) | Arxiv 2024 | `[I]` | Vulnerability-driven, Local Attention (L2-Att), Vision Transformer | [GitHub](https://github.com/10Ring/FakeFormer) |


⬆ [Back to Top](#contents)

---

## Competitions

| Competition | Link | Year | Info |
| :---------- | :--- | :--- | :--- |
| Robust AIGC Detection | [NTIRE 2026 Robust AI-Generated Image Detection in the Wild](https://www.codabench.org/competitions/12761/#/pages-tab) | 2026 | No restrictions on training data. <br> Evaluate ROC AUC metrics on robust samples. |
| Robust Deepfake Detection | [NTIRE 2026 Robust Deepfake Detection Challenge](https://www.codabench.org/competitions/12795/) | 2026 | No restrictions on training data. |
| The 6th Face Anti-spoofing Challenge | [The 6th Face Anti-Spoofing: Unified Physical-Digital Attacks Detection@ICCV2025](https://codalab.lisn.upsaclay.fr/competitions/22915) | 2025 | No external data or pre-trained models allowed. <br> Limited to a single DL model with under 100G FLOPs. |
| Detect AI vs. Human-Generated Images | [2025 Women in AI (WAI) Kaggle Challenge](https://www.kaggle.com/competitions/detect-ai-vs-human-generated-images) | 2025 | Paired dataset of authentic and AI-generated images |
| The 5th Face Anti-spoofing Challenge | [5th Chalearn Face Anti-spoofing Workshop and Challenge@CVPR2024](https://sites.google.com/view/face-anti-spoofing-challenge/welcome/challengecvpr2024) | 2024 | UniAttackData+ for unified physical and digital attack detection. |

⬆ [Back to Top](#contents)

---

## Practical Detection Tools

- **Hive Moderation** - [Website](https://thehive.ai/demos/ai-generated-content-detection)
- **Tencent Zhuque AI Detection Assistant** - [Website](https://matrix.tencent.com/ai-detect/ai_gen_txt)
- **AI or Not** - [Website](https://www.aiornot.com/)
- **Illuminarty** - [Website](https://app.illuminarty.ai/)
- **Winston AI** - [Website](https://gowinston.ai/ai-image-detector/)
- **Is it AI?** - [Website](https://isitai.com/ai-image-detector)
- **中科睿鉴 (Zhongke Ruijian)** - 微信小程序搜索 **睿鉴AI**

⬆ [Back to Top](#contents)

---

## 🏢 About Our Team
We are the **Content Security Intelligence** Team under **Ant Group - Machine Intelligence**. We are responsible for developing comprehensive content security and risk-mitigation capabilities for the Ant Group ecosystem, bridging the gap between rapidly evolving technologies and the urgent need for digital trust.

### Why We Do It
In an era where synthetic media is increasingly sophisticated and pervasive, our research serves as a critical line of defense. By advancing AIGC detection technologies, we aim to:
*   **Safeguard Digital Integrity:** We provide essential defense mechanisms to protect the authenticity of visual content and combat the spread of misinformation in the digital space.
*   **Empower Trust:** Our solutions ensure the public can distinguish between genuine and synthetic media, fostering a more transparent and trustworthy digital ecosystem.
*   **Industrial Application & Impact:** We provide robust, scalable aigc detection solutions for Ant Group’s diverse content platforms, including  **[Lingguang](https://www.lingguang.com/chat)**, **[Jingtan](https://jingtanbusiness.antgroup.com/index)**, and many others.

### 🤝 Collaborators
We are honored to collaborate with esteemed researchers and scholars in the field of AI and Computer Vision. We deeply value these academic partnerships that drive our innovation:

*   **Prof. Jun Wan (万军)** | [CASIA](http://www.ia.cas.cn/) & [UCAS](https://www.ucas.ac.cn/)
    - *Research Interests:* Biometrics, Face Anti-spoofing, Gesture Recognition, and Computer Vision.
    - [[Homepage]](https://people.ucas.edu.cn/~jwan)
*   **Prof. Jianfu Zhang (张健夫)** | [Shanghai Jiao Tong University](https://www.sjtu.edu.cn/)
    - *Research Interests:* Computer Vision, Pattern Recognition, and Image/Video Analysis & Synthesis.
    - [[Homepage]](https://www.cs.sjtu.edu.cn/jiaoshiml/zhangjianfu.html)
*   **Prof. Zhuosheng Zhang (张倬胜)** | [Shanghai Jiao Tong University](https://www.sjtu.edu.cn/)
    - *Research Interests:* Natural Language Processing, Large Language Models, and Multi-modal Learning.
    - [[Homepage]](https://www.cs.sjtu.edu.cn/jiaoshiml/zhangzhuosheng.html)

### 📝 Academic Publications
*   **VideoVeritas: AI-Generated Video Detection via Perception Pretext Reinforcement Learning** | *(Submitted), 2026*
    -   *Highlights:* Detected AI-generated videos using perception pretext reinforcement learning to capture temporal inconsistencies.
    -   [[Paper]](https://arxiv.org/pdf/2602.08828) [[Code]](https://github.com/EricTan7/VideoVeritas)
*   **Locate-Then-Examine: Grounded Region Reasoning Improves Detection of AI-Generated Images** | *CVPR'26, 2026*
    -   *Highlights:* Improved detection accuracy through a two-stage approach of localizing suspicious regions followed by detailed examination.
    -   [[Code]](https://github.com/Gennadiyev/LocateThenExamine)
*   **GAMMA: Generalizable Alignment via Multi-task and Manipulation-Augmented Training for AI-Generated Image Detection** | *ICASSP'26, 2026*
    -   *Highlights:* Enhanced generalization through multi-task learning and manipulation-augmented training strategies.
    -   [[Paper]](https://arxiv.org/pdf/2509.10250)
*   **FakeXplain: AI-Generated Image Detection via Human-Aligned Grounded Reasoning** | *ICLR'26, 2026*
    -   *Highlights:* Detected AI-generated images through human-aligned grounded reasoning, providing interpretable visual evidence.
    -   [[Paper]](https://openreview.net/pdf?id=UcpTOa8OnG) [[Code]](https://github.com/Gennadiyev/FakeXplain)
*   **Veritas: Generalizable deepfake detection via pattern-aware reasoning** | *ICLR'26 Oral, 2026*
    -   *Highlights:* Achieved generalizable deepfake detection through pattern-aware reasoning, improving robustness across diverse manipulation types.
    -   [[Paper]](https://arxiv.org/pdf/2508.21048) [[Code]](https://github.com/EricTan7/Veritas)
*   **Generalizable and Adaptive Continual Learning Framework for AI-generated Image Detection** | *IEEE TMM, 2025*
    -   *Highlights:* Proposed a continual learning framework that adapts to new generative models while mitigating catastrophic forgetting.
    -   [[Paper]](https://arxiv.org/pdf/2601.05580)
*   **Towards explainable fake image detection with multi-modal large language models** | *ACM MM'25, 2025*
    -   *Highlights:* Leveraged multi-modal large language models to provide human-interpretable explanations for fake image detection.
    -   [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3746027.3755421)
*   **WildFake: A Large-scale Challenging Dataset for AI-Generated Images Detection** | *AAAI'25 Oral, 2024*
    -   *Highlights:* Introduced the largest and most comprehensive AIGC image dataset at the time, providing a challenging benchmark for detection models.
    -   [[Paper]](https://arxiv.org/pdf/2402.11843)

### 🏆 Competition Achievements
*   **1st Place Winner** | *NTIRE 2026 Robust AI-Generated Image Detection in the Wild Challenge*
    -   Secured the top rank in ROC AUC for delivering superior performance in large-scale, real-world AI-generated image detection.
    -   [[Challenge Website]](https://www.codabench.org/competitions/12761/#/pages-tab)
*   **1st Place Winner** | *ICCV 2025 VQualA Challenge - Image Super-Resolution Generated Content Quality Assessment, 2025*
    -   Achieved top performance in the VQualA 2025 challenge focused on assessing the quality of super-resolution generated content.
    -   [[Paper 1]](https://openaccess.thecvf.com/content/ICCV2025W/VQualA/papers/Li_VQualA_2025_Challenge_on_Image_Super-Resolution_Generated_Content_Quality_Assessment_ICCVW_2025_paper.pdf) [[Paper
2]](https://openaccess.thecvf.com/content/ICCV2025W/VQualA/papers/Li_Hybrid_Vision_Transformer_and_Convolutional_Neural_Network_for_Super-Resolution_Image_ICCVW_2025_paper.pdf)
*   **1st Place Winner** | *CVPR 2024 Face Anti-Spoofing Challenge, 2024*
    -   Secured first place in the prestigious Face Anti-Spoofing Challenge at CVPR 2024, demonstrating state-of-the-art detection capabilities.
    -   [[Challenge Website]](https://sites.google.com/view/face-anti-spoofing-challenge/welcome/challengecvpr2024)

### 🛠️  Open-Source Resources
*   **WildFake** - A large and comprehensive AIGC image detection dataset.
    -   [[ModelScope]](https://modelscope.cn/datasets/hy2628982280/WildFake)
*   **GenVideo** - A large and comprehensive AIGC video detection dataset.
    -   [[ModelScope]](https://modelscope.cn/datasets/cccnju/Gen-Video)
*   **HydraFake** - A large-scale challenging dataset for AI-generated image detection.
    -   [[ModelScope]](https://www.modelscope.cn/datasets/EricTanh/HydraFake)
*   **MintVid** - A comprehensive video dataset for AIGC detection research.
    -   [[ModelScope]](https://www.modelscope.cn/datasets/EricTanh/MintVid)

### ✉️ Contact Us
For questions or collaborations, please contact:

- Zijian Yu: yuzijian.yzj@antgroup.com
- Hao Tan: tanhao2023@ia.ac.cn
- Jun Lan: yelan.lj@antgroup.com

⬆ [Back to Top](#contents)

---

### Star History

<a href="https://www.star-history.com/?repos=ant-research%2FAwesome-AIGC-Image-Video-Detection&type=date&logscale=&legend=top-left">
 <picture>
   <source media="(prefers-color-scheme: dark)" srcset="https://api.star-history.com/chart?repos=ant-research/Awesome-AIGC-Image-Video-Detection&type=date&theme=dark&legend=top-left" />
   <source media="(prefers-color-scheme: light)" srcset="https://api.star-history.com/chart?repos=ant-research/Awesome-AIGC-Image-Video-Detection&type=date&legend=top-left" />
   <img alt="Star History Chart" src="https://api.star-history.com/chart?repos=ant-research/Awesome-AIGC-Image-Video-Detection&type=date&legend=top-left" />
 </picture>
</a>

---
