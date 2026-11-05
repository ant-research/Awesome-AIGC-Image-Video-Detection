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
    - [Supervised General Detectors](#supervised-general-detectors)
    - [Video Spatiotemporal Modeling](#video-spatiotemporal-modeling)
    - [Training-Free / Zero-Shot](#training-free--zero-shot)
    - [Frequency-Domain & Low-Level Artifacts](#frequency-domain--low-level-artifacts)
    - [Continual & Incremental Learning](#continual--incremental-learning)
    - [Related & Other](#related--other)
- [Competitions](#competitions)
- [Practical Detection Tools](#practical-detection-tools)
- [About Our Team](#-about-our-team)

---

## 🔥 Hot Events

> Last updated: 2026-11-05

- 2026-11-02 · [Axios traces the use of deepfake ads in US Senate campaigns](https://www.axios.com/newsletters/axios-indianapolis-02a5f43f-3367-4882-98ee-a39a593eb415)
- 2026-10-28 · [抖音公布治理滥用 AI 的恶意营销账号案例](https://news.fznews.com.cn/gngj/20261029/41ilx2u53c.shtml)
- 2026-10-28 · [AP investigates manipulated videos impersonating real people in Senate races](https://apnews.com/article/c52f2c1720a0bb1ea86545d260aaf969)
- 2026-10-27 · [UK police report £24.3 million in losses from AI-enabled investment scams](https://www.cityoflondon.police.uk/news/city-of-london/news/2026/october/report-fraud-warning-after-24.3-million-stolen-through-ai-enabled-investment-endorsement-schemes/)
- 2026-10-27 · [DeepMind introduces Genie 4](https://deepmind.google/blog/genie-4-a-new-generation-of-world-simulation/)
- 2026-10-25 · [央视调查 AI 换脸明星带货](https://news.cctv.com/2026/10/25/ARTIGlfSeulXszyO6KXfdod3261025.shtml)
- 2026-10-22 · [Brennan Center repeats election-image tests on six generators](https://www.brennancenter.org/our-work/analysis-opinion/major-ai-models-are-more-willing-ever-create-fake-election-images)
- 2026-10-21 · [Teacher awarded damages over deepfake image edits](https://news.sbs.co.kr/english/article.do?news_id=N1008807755)
- 2026-10-10 · [Nikon withdraws microscopy video prize after reviewing AI use](https://www.abc.net.au/news/2026-10-10/winner-of-nikon-small-world-in-motion-competition-ai-generated/107251164)
- 2026-09-15 · [Apple introduces Reference Image for verifiable photography](https://security.apple.com/blog/apple-reference-image/)
- 2025-12-18 · [Gemini adds SynthID checks for Google AI video](https://blog.google/innovation-and-ai/products/verify-google-ai-videos-gemini-app/)
- 2025-10-29 · [Fact-checkers trace viral Hurricane Melissa footage to an AI-labelled upload](https://fullfact.org/environment/hurricane-melissa-video-from-above-ai/)
- 2025-09-01 · [《人工智能生成合成内容标识办法》施行](https://www.cac.gov.cn/2025-03/14/c_1743654684782215.htm)
- [⭐️ 蚂蚁安全实验室获CVPR26 AIGC图像检测挑战赛冠军](https://mp.weixin.qq.com/s/xlvP_rkyaLD0Pfp4g3Jwdw)
- [⭐️ 蚂蚁安全实验室夺冠全球人脸防伪检测挑战赛](https://mp.weixin.qq.com/s/ZZMep9ETEavC99N-GyfRBQ)

**[View all hot events →](./docs/hot-events.md)**

⬆ [Back to Top](#contents)

---

## Benchmarks & Datasets

> **Modality Legend:** `[I]` Image | `[V]` Video | `[M]` Multi-modal

> **Annotation Type Legend:** 
> `Au`: Authenticity | `Ex`: Explainability | `Lo`: Localization

| Benchmark | Paper | Venue & Year | Modality | Notes | Real Source | Fake Source/Generator | Annotation | Scale | Download |
| :-------- | :---- | :----------- | :------- | :------ | :---------- | :-------------------- | :--------- | :---- | :------- |
| WildAIGC-Bench | [WildAIGC-Bench: Can AI Image Detectors Handle the Wild? A Benchmark of Generated and Edited Images in Online Circulation](https://arxiv.org/abs/2610.28087) | Arxiv 2026 | `[I]` | In-the-Wild AIGI Benchmark, Human-Verified News Labels, Online-Circulation Artifacts | 638 source-reviewed real photographs (v3) | Generated/edited images circulating on news, fact-checking and social-media sites | `Au` | 1,238 (600 AI + 638 real; v3) | [WildAIGC-Bench](https://huggingface.co/datasets/yuzj1997yzj/WildAIGC-Bench) <br> [Code](https://github.com/YuZijian/WildAIGC-Bench) <br> [Project](https://yuzijian.github.io/WildAIGC-Bench/) |
| DF26 | [DF26: We Cannot Tell Fake From Real Anymore](https://arxiv.org/abs/2609.07369) | Arxiv 2026 | `[V]` | Modern-Generator AIGV Benchmark, Public-Speaking Scenarios, Evaluation-Only Closed Subset | OpenVid-1M, TalkingCelebs, MAVOS-DD | 7 recent T2V/I2V models: Wan2.6, Veo 3.1, Grok Imagine 1.0, Kling 3.0 (closed); Wan2.2-A14B, HunyuanVideo 1.5, LTX 2.3 (open) | `Au` | 2.7K (271 real + 2,420 fake, 1280×720) | [DF26](https://huggingface.co/datasets/DF26/DF26) (controlled access) |
| DailyBench | [DailyBench: A Unified Benchmark for AI-Generated and Manipulated Images from Modern Generative Models](https://arxiv.org/abs/2607.24016) | Arxiv 2026 (v3 2026-09-01) | `[I]` | Unified AI-Generated Image Detection Testbed, FakeBench + ManipulationBench, Per-Generator Pairs | LAION-Aesthetics V2 | T2I: SD3.5-Large, FLUX.1, FLUX.2, Qwen-Image-2512, Z-Image, Nano Banana 2, GPT-Image 2; Edit: FLUX-Fill (random/object mask), FLUX.2-klein-9B, Qwen-Image-Edit-2511, Step1X-Edit-v1p2 | `Au` | 270K（v3：FakeBench ≈185K + ManipulationBench ≈75K） | [DailyBench](https://modelscope.cn/datasets/WhiteJiang/DailyBench) <br> [Project](https://dailybench.github.io/) |
| FraudBench | [FraudBench: A Multimodal Benchmark for Detecting AI-Generated Fraudulent Refund Evidence](https://arxiv.org/pdf/2605.08820) | Arxiv 2026 | `[M]` | Fraudulent Refund Detection (ECommerce) | User-review images from e-commerce, food delivery and travel services | 12 editing and generation models (paper v2) | `Au` | — | [FraudBench](https://huggingface.co/datasets/TristanYan/FraudBench) |
| ActivityForensics | [ActivityForensics: A Comprehensive Benchmark for Localizing Manipulated Activity in Videos](https://openaccess.thecvf.com/content/CVPR2026/html/Bao_ActivityForensics_A_Comprehensive_Benchmark_for_Localizing_Manipulated_Activity_in_Videos_CVPR_2026_paper.html) | CVPR 2026 | `[V]` | Action-level AIGC in videos | — | — | `Au`, `Lo` (temporal) | 6K | [Dataset](https://huggingface.co/datasets/ActivityForensics/ActivityForensics) |
| GenVidBench | [GenVidBench: A 6-Million Benchmark for AI-Generated Video Detection](https://arxiv.org/pdf/2501.11340) | AAAI 2026 | `[V]` | — | — | — | `Au` | 6.78M | [GenVidBench](https://huggingface.co/datasets/jian-0/GenVidBench/tree/main) |
| Chameleon | [A Sanity Check for AI-Generated Image Detection](https://arxiv.org/abs/2406.19435) | ICLR 2025 | `[I]` | — | Unsplash | Midjourney, DALLE-3, Stable Diffusion (various LoRA fine-tuned) | `Au` | 26K | [Author access instructions](https://github.com/shilinyan99/AIDE) (email request; noncommercial use) |
| WildFake | [WildFake: A Large-scale Challenging Dataset for AI-Generated Images Detection](https://arxiv.org/pdf/2402.11843) | AAAI 2025 | `[I]` | — | — | — | `Au` | 3.7M | [WildFake](https://modelscope.cn/datasets/hy2628982280/WildFake/summary) |
| DF40 | [DF40: Toward Next-Generation Deepfake Detection](https://arxiv.org/abs/2406.13495) | NeurIPS 2024 | `[I]` `[V]` | — | — | — | `Au` | 0.1M+ videos, 1M+ images | [DF40](https://github.com/YZY-stack/DF40) |
| GenImage | [GenImage: A Million-Scale Benchmark for Detecting AI-Generated Image](https://proceedings.neurips.cc/paper_files/paper/2023/file/f4d4a021f9051a6c18183b059117e8b5-Paper-Datasets_and_Benchmarks.pdf) | NeurIPS 2023 | `[I]` | — | ImageNet, Wukong | MidJourney, SDv1.4, SDv1.5, ADM, GLIDE, VQDM, BigGAN | `Au` | 2.7M | [GenImage](https://drive.google.com/drive/folders/1jGt10bwTbhEZuGXLyvrCuxOI0cBqQ1FS) |

**[View all benchmarks & datasets →](./docs/benchmarks-and-datasets.md)**

⬆ [Back to Top](#contents)

---

## Research Papers

> **💡 Note:** Papers are sorted by year (descending) within each category. <br>
> **Modality Legend:** `[I]` Image | `[V]` Video | `[M]` Multi-modal <br>
> **Category Layout:** Top level is split into **MLLM-Based** (MLLM-powered detection) and **Classification-Based** (compact/traditional classifiers). Classification-Based is further organized into six subcategories. When a paper fits multiple subcategories, the priority is: **Training-Free/Zero-Shot > Continual/Incremental > Video Spatiotemporal > Frequency/Low-Level Artifacts > Supervised General**.

### MLLM-Based
*This category focuses on utilizing Multimodal Large Language Models (MLLMs) like GPT-4V, LLaVA, or Qwen-VL to detect AI-generated content. These methods often provide natural language explanations (explainability) alongside binary detection.*

| Title | Venue & Year | Modality | Highlights/Keywords | Code |
| --- | --- | --- | --- | --- |
| [Agentic Tool-Augmented Reasoning for Explainable Image Forgery Detection](https://arxiv.org/abs/2609.39066) | ACM MM 2026 (Oral) | `[I]` | ATAR, 22 Forensic Tools across 7 Domains, Dual-Stream Forensic Reasoning, Forensics Curriculum Learning | N/A |
| [Evidence-Guided Detection, Localization and Explanation for Text-Centric Image Forensics](https://arxiv.org/abs/2609.02097) | ACM MM 2026 Challenge | `[I]` | Detector-Localizer-Reasoner Cascade, Iterative Difficulty-Aware Mining, Report-Mask Consistency | [GitHub](https://github.com/peifengLiu42/ACMMM26-evidence-guided-detector-localizer-reasoner-system) |
| [AGIDefect-4K: A Richly Annotated Dataset for AI-Generated Image Defect Detection, Localization and Explanation](https://arxiv.org/abs/2608.20713) | ACM MM 2026 | `[I]` | AGIDefect-4K Dataset, Hierarchical Defect Annotation, MLLM Baseline (AGIDA) | [GitHub](https://github.com/sxfly99/AGIDefect-4K) |
| [PATE-Forensics: Perception-as-Tool for Explainable Deepfake Forensics with General-Purpose MLLMs](https://arxiv.org/abs/2608.18573) | IJCAI 2026 Workshop | `[I]` | Perception-as-Tool, DINOv3 Forensic Perception Tool, General-Purpose MLLM Explanation | [GitHub](https://github.com/yqli00000/PATE-Forensics) |
| [VidForensics-M1: Meta-Detection Reinforcement Learning with Verifiable Temporal Grounding for AI-Generated Video Forensics](https://arxiv.org/abs/2608.11201) | Arxiv 2026 | `[V]` | Meta-Detection RL, Verifiable Temporal Grounding, Evidence-Guided Reward Redistribution | N/A |
| [TranX-Adapter: Bridging Artifacts and Semantics within MLLMs for Robust AI-generated Image Detection](https://arxiv.org/abs/2602.21716) | ICML 2026 | `[I]` | Artifact feature and Semantic feature fusion | [GitHub](https://github.com/DreamMr/TranX-Adapter) |
| [VideoVeritas: AI-Generated Video Detection via Perception Pretext Reinforcement Learning](https://proceedings.mlr.press/v306/tan26b.html) | ICML 2026 | `[V]` | Perception Pretext RL, Fact-based Reasoning, MintVid Dataset | [GitHub](https://github.com/EricTan7/VideoVeritas) |
| [Veritas: Generalizable deepfake detection via pattern-aware reasoning](https://arxiv.org/pdf/2508.21048) | ICLR 2026(Oral) | `[I]` | Pattern-aware Reasoning, HydraFake Dataset | [Github](https://github.com/EricTan7/Veritas) |
| [VidGuard-R1: AI-Generated Video Detection and Explanation via Reasoning MLLMs and RL](https://arxiv.org/abs/2510.02282) | ICLR 2026 | `[V]` | Multi-stage RL (GRPO), Time Artifacts, Video Detection Dataset | [GitHub](https://github.com/kyoungjunpark/VidGuard-R1) |
| [GenVideoLens: Where LVLMs Fall Short in AI-Generated Video Detection?](https://arxiv.org/pdf/2603.18625) | Arxiv 2026 | `[V]` | GenVideoLens benchmark | N/A |
| [BusterX++: Towards Unified Cross-Modal AI-Generated Content Detection and Explanation with MLLM](https://www.alphaxiv.org/pdf/2507.14632) | Arxiv 2025 | `[M]` | RL Post-training, Cross-Modal, Thinking Reward Mechanism | [Github](https://github.com/l8cv/BusterX) |
| [Spot the Fake: Large Multimodal Model-Based Synthetic Image Detection with Artifact Explanation](https://arxiv.org/pdf/2503.14905) | NeurIPS 2025 | `[I]` | FakeClue Dataset, Fine-grained Artifact Clues, Artifact Explanation | [GitHub](https://github.com/opendatalab/FakeVLM) |
| [LEGION: Learning to Ground and Explain for Synthetic Image Detection](https://arxiv.org/pdf/2503.15264) | ICCV 2025 | `[I]` | SynthScars Dataset, Defender & Controller, Image Refinement | [GitHub](https://github.com/opendatalab/LEGION) |
| [SIDA: Social Media Image Deepfake Detection, Localization, and Explanation](https://arxiv.org/pdf/2412.04292) | CVPR 2025 | `[I]` | SID-Set, Mask Prediction, Social Media Context | [Github](https://github.com/hzlsaber/SIDA) |
| [FakeShield: Explainable Image Forgery Detection and Localization via Multi-modal Large Language Models](https://arxiv.org/pdf/2410.02761) | ICLR 2025 | `[I]` | Explainable IFDL, Domain Tag-guided, Multi-modal Localization | [GitHub](https://github.com/zhipeixu/FakeShield) |


### Classification-Based
*This category includes supervised learning approaches that train neural networks (CNNs, ViTs, VFMs, etc.) specifically to classify authentic vs. AI-generated content. They usually focus on robustness, generalization, and feature extraction. It is organized into six subcategories: Supervised General Detectors, Video Spatiotemporal Modeling, Training-Free / Zero-Shot, Frequency-Domain & Low-Level Artifacts, Continual & Incremental Learning, and Related & Other.*

#### Supervised General Detectors
*Trainable classifiers and backbones (CNNs, ViTs, vision foundation models, CLIP-based adapters, few-shot and prompt-based methods) for general-purpose detection.*

| Title | Venue & Year | Modality | Highlights/Keywords | Code |
| --- | --- | --- | --- | --- |
| [Less Supervision, Better Generalization: Weakly Supervised Fake Region Localization in Diffusion-Edited Images](https://arxiv.org/abs/2609.36882) | NeurIPS 2026 | `[I]` | ReGFLoW, First Weakly Supervised Diffusion-Edit Localization, Image-Level Labels Only, Diffusion Reconstruction Error as Dense Guidance, Artifact-Centric MIL | N/A |
| [LoRC: Detecting AI-Generated Images via Low-Rank Collapse in Semantic Residuals](https://arxiv.org/abs/2608.20882) | ECCV 2026 (Spotlight) | `[I]` | Low-Rank Collapse Signature, Semantic-Residual Decoupling, Cross-model Generalization | N/A |
| [Harnessing CLIP and DINO: An Uncertainty-Aware Cascaded Fusion Network for Generalizable Deepfake Image Detection](https://arxiv.org/abs/2609.07670) | Arxiv 2026 | `[I]` | UCF-Net, CLIP Semantic + DINO Structural Priors, Layer-wise Expert Aggregation, Entropy-based Uncertainty Fusion, 4M-image Unified Benchmark, Cross-generator Evaluation | [GitHub](https://github.com/XavierJiezou/UCF-Net) |
| [Fleet: Few Shots Lead Effective AI-generated Image Detection](https://arxiv.org/abs/2606.31082) | ICML 2026 | `[I]` | Few-shot Adaptation, Routing Correction, Treasure Benchmark | [GitHub](https://github.com/ICTMCG/Fleet) |
| [PGC: Peak-Guided Calibration for Generalizable AI-Generated Image Detection](https://arxiv.org/pdf/2605.21207) | ICML 2026 | `[I]` | Peak-Guided Calibration, CommGen15 Dataset | [GitHub](https://github.com/xiaoyu6868/PGC) |
| [Reduce the Artifacts Bias for More Generalizable AI-Generated Image Detection](https://arxiv.org/pdf/2605.14486) | Arxiv 2026 | `[I]` | Bias-free Training | [GitHub](https://github.com/liyih/SEF_AIGC_detection) |
| [No Pixel Left Behind: A Detail-Preserving Architecture for Robust High-Resolution AI-Generated Image Detection](https://arxiv.org/pdf/2508.17346) | ICLR 2026 | `[I]` | Detail-preserving dual-path architecture, Multi-task learning, HiRes-50K benchmark | N/A |
| [DINO-Detect: A Simple yet Effective Framework for Blur-Robust AI-Generated Image Detection](https://arxiv.org/pdf/2511.12511) | Arxiv 2025 | `[I]` | Blur Robustness, Knowledge Distillation, DINOv3 | [Github](https://github.com/JiaLiangShen/Dino-Detect-for-blur-robust-AIGC-Detection) |
| [A Bias-Free Training Paradigm for More General AI-generated Image Detection](https://arxiv.org/pdf/2412.17671) | CVPR 2025 | `[I]` | Bias-Free, Semantic Alignment, Stable Diffusion Self-conditioning | [Github](https://github.com/grip-unina/B-Free) |
| [Forensics Adapter: Adapting CLIP for Generalizable Face Forgery Detection](https://arxiv.org/pdf/2411.19715) | CVPR 2025 | `[I]` | CLIP, Blending Boundaries, Forgery-aware Prompt Learning | [Github](https://github.com/OUC-VAS/ForensicsAdapter) |

#### Video Spatiotemporal Modeling
*Methods that exploit temporal inconsistencies, motion patterns, and spatiotemporal artifacts in AI-generated videos.*

| Title | Venue & Year | Modality | Highlights/Keywords | Code |
| --- | --- | --- | --- | --- |
| [Temporal Slice Learning for AI-Generated Video Detection with 400$\times$ Fewer FLOPs](https://arxiv.org/abs/2610.35148) | NeurIPS 2026 | `[V]` | TSC-Net, Temporal Slice Representation, Frequency-Aware Slice Consistency Learning, Task-Driven Slice Localization, Lightweight Transformer (1.7M Params), 400$\times$ Fewer FLOPs / 3.6$\times$ Faster Inference, GenVideo & AI-Artist Benchmark | N/A |
| [Mind the Rift: Cross-Scale Coupling Mismatch for AI-Generated Video Detection](https://arxiv.org/abs/2609.00742) | ACM MM 2026 | `[V]` | Cross-Scale Coupling Mismatch, Macro Temporal Dynamics vs. Pixel-Level Residuals, Persistent Homology, Encoder-Agnostic | [GitHub](https://github.com/Litsay/RIFT) |
| [MotionPhys: Detecting AI-Generated Videos via Physical Consistency of Optical-Flow Trajectories](https://arxiv.org/abs/2608.20770) | Arxiv 2026 | `[V]` | Physical Motion Consistency, Sparse Optical-Flow Trajectories, Multi-scale Geometric Evolution | N/A |
| [Dataset Biases and Shortcut Learning in Motion-Based AI-Generated Video Detection](https://arxiv.org/abs/2607.00948) | Arxiv 2026 | `[V]` | Motion Bias Analysis, Preprocessing/Sampling Bias, Frequency-based Comparison | N/A |
| [G2VD: Generalizable AI-Generated Video Detection via Counterfactual Intervention and Causal Disentanglement](https://arxiv.org/abs/2607.04607) | Arxiv 2026 | `[V]` | Counterfactual Intervention, Causal Disentanglement, Cross-domain Generalization | Not publicly accessible |
| [CMTA: Leveraging Cross-Modal Temporal Artifacts for Generalizable AI-Generated Video Detection](https://arxiv.org/pdf/2605.00630) | Arxiv 2026 | `[V]` | Cross-Modal Temporal Artifacts, Video Detection | N/A |
| [DeMamba: AI-Generated Video Detection on Million-Scale GenVideo Benchmark](https://doi.org/10.1007/s11432-024-4894-0) · [arXiv](https://arxiv.org/pdf/2405.19707) | Science China Information Sciences 2026 | `[V]` | Mamba, State Space Model, Long-range Spatiotemporal Inconsistency | [GitHub](https://github.com/chenhaoxing/DeMamba) |
| [Seeing What Matters: Generalizable AI-generated Video Detection with Forensic-Oriented Augmentation](https://arxiv.org/pdf/2506.16802) | NeurIPS 2025 | `[V]` | Wavelet-band Augmentation, Forensic Frequency Artifacts, Single-generator Generalization | [GitHub](https://github.com/grip-unina/WaveRep-SyntheticVideoDetection) |
| [AI-Generated Video Detection via Perceptual Straightening](https://arxiv.org/pdf/2507.00583) | NeurIPS 2025 | `[V]` | Perceptual Straightening, DINOv2, Temporal Curvature | [GitHub](https://github.com/ChristianInterno/ReStraV) |
| [Physics-Driven Spatiotemporal Modeling for AI-Generated Video Detection](https://arxiv.org/pdf/2510.08073) | NeurIPS 2025 | `[V]` | Normalized Spatiotemporal Gradient (NSG), Maximum Mean Discrepancy (MMD) | [Github](https://github.com/ZSHsh98/NSG-VD) |

#### Training-Free / Zero-Shot
*Methods that detect AI-generated content without additional training on detection data.*

| Title | Venue & Year | Modality | Highlights/Keywords | Code |
| --- | --- | --- | --- | --- |
| [Frozen DINO Localizes Image Edits Without a Localizer](https://arxiv.org/abs/2608.18968) | Arxiv 2026 | `[I]` | Training-free, Frozen DINO Patch-token Drift, Haar Perturbation, Edit Localization | [GitHub](https://github.com/VishalJ99/trail-image-edit-localization) |
| [SPLIT: Training-Free AI-Generated and Partially Edited Video Detection via Spatial Patch-Level Incoherence and Temporal Roughness](https://arxiv.org/abs/2607.02886) | ECCV 2026 | `[V]` | Training-free, Patch-level Incoherence, Temporal Roughness, Ultra-low FPR | [GitHub](https://github.com/mldljyh/SPLIT) |
| [Training-free Detection of Generated Videos via Spatial-Temporal Likelihoods](https://arxiv.org/pdf/2603.15026) | CVPR 2026 | `[V]` | Training-free, Zero-shot, Spatial-Temporal Likelihoods, ComGenVid Dataset | [GitHub](https://github.com/OmerBenHayun/STALL) |

#### Frequency-Domain & Low-Level Artifacts
*Methods based on spectral analysis, quantization/upsampling traces, and other low-level generative artifacts.*

| Title | Venue & Year | Modality | Highlights/Keywords | Code |
| --- | --- | --- | --- | --- |
| [Dual Data Alignment Makes AI-Generated Image Detector Easier Generalizable](https://arxiv.org/pdf/2505.14359) | NeurIPS 2025 (Spotlight) | `[I]` | Dual-domain Alignment, Frequency-level Bias, VAE Reconstruction | [GitHub](https://github.com/roy-ch/Dual-Data-Alignment) |
| [D3QE: Learning Discrete Distribution Discrepancy-aware Quantization Error for Autoregressive-Generated Image Detection](https://openaccess.thecvf.com/content/ICCV2025/html/Zhang_D3QE_Learning_Discrete_Distribution_Discrepancy-aware_Quantization_Error_for_Autoregressive-Generated_Image_ICCV_2025_paper.html) | ICCV 2025 | `[I]` | Discrete Distribution Discrepancy-aware Transformer, Vector Quantized Variational AutoEncoder | [Github](https://github.com/Zhangyr2022/D3QE) |
| [Any-Resolution AI-Generated Image Detection by Spectral Learning](https://arxiv.org/pdf/2411.19417) | CVPR 2025 | `[I]` | Spectral Context Attention, Frequency Reconstruction, OOD Detection | [Github](https://github.com/kartyg23/spai) |
| [Frequency-Aware Deepfake Detection: Improving Generalizability through Frequency Space Domain Learning](https://ojs.aaai.org/index.php/AAAI/article/view/28310) | AAAI 2024 | `[I]` | Frequency Domain, FFT, Frequency Conv Layer (FCL), Lightweight | [GitHub](https://github.com/chuangchuangtan/FreqNet-DeepfakeDetection) |
| [Rethinking the Up-Sampling Operations in CNN-based Generative Network for Generalizable Deepfake Detection](https://openaccess.thecvf.com/content/CVPR2024/html/Tan_Rethinking_the_Up-Sampling_Operations_in_CNN-based_Generative_Network_for_Generalizable_CVPR_2024_paper.html) | CVPR 2024 | `[I]` | Neighboring Pixel Relationships, Generalized Structural Artifacts | [Github](https://github.com/chuangchuangtan/NPR-DeepfakeDetection) |

#### Continual & Incremental Learning
*Methods that keep adapting detectors to evolving generators without catastrophic forgetting.*

| Title | Venue & Year | Modality | Highlights/Keywords | Code |
| --- | --- | --- | --- | --- |
| [Preserving Knowledge across Space and Time for Continual Video Deepfake Detection](https://arxiv.org/abs/2609.03446) | ECCV 2026 | `[V]` | Modality-Specific Frequency Distillation, Spatial/Temporal/Spatiotemporal Decomposition, Cross-Modality Decorrelation | [GitHub](https://github.com/rama0126/MSFD) |
| [Automated In-the-Wild Data Collection for Continual AI Generated Image Detection](https://doi.org/10.1145/3810988.3812662) · [arXiv](https://arxiv.org/pdf/2605.02567) | MAD 2026 (ACM Workshop) | `[I]` | Continual Learning, Continual Data Collection | [GitHub](https://github.com/mever-team/WildFC) |
| [IncreFA: Breaking the Static Wall of Generative Model Attribution](https://openaccess.thecvf.com/content/CVPR2026/html/Qin_IncreFA_Breaking_the_Static_Wall_of_Generative_Model_Attribution_CVPR_2026_paper.html) | CVPR 2026 | `[I]` | Incremental Learning, Generative Model Attribution | [GitHub](https://github.com/Ant0ny44/IncreFA) |
| [SAIDO: Generalizable Detection of AI-Generated Images via Scene-Aware and Importance-Guided Dynamic Optimization in Continual Learning](https://arxiv.org/pdf/2512.00539) | CVPR 2026 | `[I]` | Scene-aware optimization, Continual learning | [GitHub](https://github.com/edu-yinzhaoxia/SAIDO-CVPR-2026) |
| [Generalizable and Adaptive Continual Learning Framework for AI-generated Image Detection](https://arxiv.org/pdf/2601.05580) | TMM 2026 | `[I]` | Continual Learning, Kronecker-Factored Approximate Curvature | [GitHub](https://github.com/Mark-Dou/AIGIDetectionBenchmark) |

#### Related & Other
*Papers related to AI-generated content safety (e.g., provenance/watermarking, misinformation verification) that do not fit the subcategories above.*

| Title | Venue & Year | Modality | Highlights/Keywords | Code |
| --- | --- | --- | --- | --- |
| [DF26: We Cannot Tell Fake From Real Anymore](https://arxiv.org/abs/2609.07369) | Arxiv 2026 | `[V]` | [Benchmark] 2,691 Public-Speaking Videos, 7 Modern T2V/I2V Models, Human & SOTA Detectors Near Chance, Distribution-Shift Robustness | N/A |
| [APT: Anchor-aligned Perturbations for Tamper Localization in Fully Regenerated Images](https://arxiv.org/abs/2608.30656) | ECCV 2026 | `[I]` | [Proactive Forensics] Semi-Fragile Latent Perturbation, Fully Regenerated (Inpainting) Setting, Anchor-Direction Alignment | N/A |
| [Training-Free Reconstruction-Based AI-Generated Image Detectors Are Inherently Vulnerable to Adversarial Examples](https://arxiv.org/abs/2608.16646) | ECCV 2026 Workshop | `[I]` | [Robustness Analysis] Reconstruction-based Detector Attacks, Transferable Adversarial Examples, Real-world Degradations | N/A |
| [When Seeing Is Not Believing -- A Benchmark for Search-Grounded Video Misinformation Detection](https://aclanthology.org/2026.findings-emnlp.763/) | Findings of EMNLP 2026 | `[V]` | Search-Grounded Verification, EVID-Bench, Evidence-Dependent Manipulation | N/A |
| [Robust ASIC-Based Image Authentication Using Reed-Solomon LSB Watermarking](https://github.com/Agnuxo1/Secure_image_generation_with_ASIC_signature) | Preprint 2026 | `[I]` | ASIC PoW, Hardware-bound Provenance, Reed-Solomon Watermarking | [GitHub](https://github.com/Agnuxo1/Secure_image_generation_with_ASIC_signature) |

**[View all research papers →](./docs/research-papers.md)**

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

- **美亚鉴真** - 微信小程序搜索 **美亚鉴真**
- **SiliconSignature** - [GitHub](https://github.com/Agnuxo1/Secure_image_generation_with_ASIC_signature) - Hardware-bound image authentication using ASIC PoW nonces for unforgeable provenance certification
- **EyeSift** - [Website](https://www.eyesift.com/) - Free online AI text/image/video/audio detector with detailed per-model benchmarks
- **Hive Moderation** - [Website](https://thehive.ai/demos/ai-generated-content-detection)
- **Tencent Zhuque AI Detection Assistant** - [Website](https://matrix.tencent.com/ai-detect/ai_gen_txt)
- **AI or Not** - [Website](https://www.aiornot.com/)
- **Illuminarty** - [Website](https://app.illuminarty.ai/)
- **Winston AI** - [Website](https://gowinston.ai/ai-image-detector/)
- **Is it AI?** - [Website](https://isitai.com/ai-image-detector)
- **TruthScan** - [Website](https://truthscan.com/zh)
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
*   **Veritas++: Value-aware On-Policy Distillation for Perception-Enhanced AIGI Detection** | *arXiv, 2026*
    -   *Highlights:* Strengthened fine-grained visual perception for explainable AIGI detection through perception-oriented learning and value-aware on-policy distillation.
    -   [[Paper]](https://arxiv.org/abs/2607.27113) [[Code]](https://github.com/EricTan7/VeritasPP)
*   **VideoVeritas: AI-Generated Video Detection via Perception Pretext Reinforcement Learning** | *ICML'26, 2026*
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

## Star History

<a href="https://www.star-history.com/?repos=ant-research%2FAwesome-AIGC-Image-Video-Detection&type=date&legend=top-left">
 <picture>
   <source media="(prefers-color-scheme: dark)" srcset="https://api.star-history.com/chart?repos=ant-research/Awesome-AIGC-Image-Video-Detection&type=date&theme=dark&legend=top-left&sealed_token=2BuClRf-coPk9YPAPXeYMlqzc-HCXTdEaMC-VD2C4XBrGanda3wxhpYiBvSiWAh2qbRHjtpLc-p75i-YrEok1aHHI5a3kmTkccBPgbMRZYvlaW1l-kAwrQ" />
   <source media="(prefers-color-scheme: light)" srcset="https://api.star-history.com/chart?repos=ant-research/Awesome-AIGC-Image-Video-Detection&type=date&legend=top-left&sealed_token=2BuClRf-coPk9YPAPXeYMlqzc-HCXTdEaMC-VD2C4XBrGanda3wxhpYiBvSiWAh2qbRHjtpLc-p75i-YrEok1aHHI5a3kmTkccBPgbMRZYvlaW1l-kAwrQ" />
   <img alt="Star History Chart" src="https://api.star-history.com/chart?repos=ant-research/Awesome-AIGC-Image-Video-Detection&type=date&legend=top-left&sealed_token=2BuClRf-coPk9YPAPXeYMlqzc-HCXTdEaMC-VD2C4XBrGanda3wxhpYiBvSiWAh2qbRHjtpLc-p75i-YrEok1aHHI5a3kmTkccBPgbMRZYvlaW1l-kAwrQ" />
 </picture>
</a>

---
