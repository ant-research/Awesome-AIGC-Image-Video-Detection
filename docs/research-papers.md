# Research Papers

[← Back to README](../README.md#research-papers)

## Contents

- [MLLM-Based](#mllm-based)
- [Classification-Based](#classification-based)
  - [Supervised General Detectors](#supervised-general-detectors)
  - [Video Spatiotemporal Modeling](#video-spatiotemporal-modeling)
  - [Training-Free / Zero-Shot](#training-free--zero-shot)
  - [Frequency-Domain & Low-Level Artifacts](#frequency-domain--low-level-artifacts)
  - [Continual & Incremental Learning](#continual--incremental-learning)
  - [Related & Other](#related--other)

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
| [Explainable Deepfake Detection with Feature-robust Augmentation and Evidence-grounded Explanation Optimization](https://arxiv.org/abs/2608.20913) | ACM MM 2026 | `[I]` | Feature-robust Augmentation, Mean-Teacher Consistency, Evidence-grounded Preference Optimization, Challenge Winner | [GitHub](https://github.com/oceanflowlab/EDD) |
| [PATE-Forensics: Perception-as-Tool for Explainable Deepfake Forensics with General-Purpose MLLMs](https://arxiv.org/abs/2608.18573) | IJCAI 2026 Workshop | `[I]` | Perception-as-Tool, DINOv3 Forensic Perception Tool, General-Purpose MLLM Explanation | [GitHub](https://github.com/yqli00000/PATE-Forensics) |
| [Defake-o3: From Speculative Rationales to Verifiable Evidence for Explainable AIGI Detection](https://arxiv.org/abs/2608.16259) | ACM MM 2026 | `[I]` | Interactive Visual Search, Verifier-guided Evidence Alignment, GroundFake Dataset, FakeFrontier Benchmark | N/A |
| [SPARED: Reasoning-Based AI-Generated Image Detection via Adversarially Edited Data](https://arxiv.org/abs/2608.12876) | Arxiv 2026 | `[I]` | Adversarial RL Loop, Diffusion Editor, Free-form Explanation | N/A |
| [VidForensics-M1: Meta-Detection Reinforcement Learning with Verifiable Temporal Grounding for AI-Generated Video Forensics](https://arxiv.org/abs/2608.11201) | Arxiv 2026 | `[V]` | Meta-Detection RL, Verifiable Temporal Grounding, Evidence-Guided Reward Redistribution | N/A |
| [Veritas++: Value-aware On-Policy Distillation for Perception-Enhanced AIGI Detection](https://arxiv.org/abs/2607.27113) | Arxiv 2026 | `[I]` | Value-aware On-Policy Distillation, Perception-Enhanced Reasoning | [GitHub](https://github.com/EricTan7/VeritasPP) |
| [Detecting AI-Generated Video: A Vision-Language Dual-View Survey](https://arxiv.org/abs/2607.10787) | ACL 2026 Findings | `[V]` | [Survey] Vision-Language Dual-View Taxonomy, Factual Fidelity Verification, Cross-modal Consistency | N/A |
| [TranX-Adapter: Bridging Artifacts and Semantics within MLLMs for Robust AI-generated Image Detection](https://arxiv.org/abs/2602.21716) | ICML 2026 | `[I]` | Artifact feature and Semantic feature fusion | [GitHub](https://github.com/DreamMr/TranX-Adapter) |
| [GenShield: Unified Detection and Artifact Correction for AI-Generated Images](https://arxiv.org/pdf/2605.16122) | ICML 2026 | `[I]` | Unified MLLM, Detect & Correct Artifacts | [GitHub](https://github.com/zhipeixu/GenShield) |
| [ReAlign: Generalizable Image Forgery Detection via Reasoning-Aligned Representation](https://openaccess.thecvf.com/content/CVPR2026/html/Huang_ReAlign_Generalizable_Image_Forgery_Detection_via_Reasoning-Aligned_Representation_CVPR_2026_paper.html) | CVPR 2026 | `[I]` | Reasoning-Aligned Representation, Interpretable | N/A |
| [UniGenDet: A Unified Generative-Discriminative Framework for Co-Evolutionary Image Generation and Generated Image Detection](https://arxiv.org/abs/2604.21904v1) | CVPR 2026 | `[I]` | Unified Model, Co-Evolution (Generation & Detection) | [GitHub](https://github.com/Zhangyr2022/UniGenDet) |
| [VideoVeritas: AI-Generated Video Detection via Perception Pretext Reinforcement Learning](https://proceedings.mlr.press/v306/tan26b.html) | ICML 2026 | `[V]` | Perception Pretext RL, Fact-based Reasoning, MintVid Dataset | [GitHub](https://github.com/EricTan7/VideoVeritas) |
| [Veritas: Generalizable deepfake detection via pattern-aware reasoning](https://arxiv.org/pdf/2508.21048) | ICLR 2026(Oral) | `[I]` | Pattern-aware Reasoning, HydraFake Dataset | [Github](https://github.com/EricTan7/Veritas) |
| [DF-LLaVA: Unlocking MLLMs for Synthetic Image Detection via Knowledge Injection and Conflict-Driven Self-Reflection](https://arxiv.org/pdf/2509.14957) | Arxiv 2026 | `[I]` | Knowledge Injection, Self-Reflection | N/A |
| [DocShield: Towards AI Document Safety via Evidence-Grounded Agentic Reasoning](https://arxiv.org/pdf/2604.02694) | Arxiv 2026 | `[M]` | Agentic Framework, Document Safety | N/A |
| [VidGuard-R1: AI-Generated Video Detection and Explanation via Reasoning MLLMs and RL](https://arxiv.org/abs/2510.02282) | ICLR 2026 | `[V]` | Multi-stage RL (GRPO), Time Artifacts, Video Detection Dataset | [GitHub](https://github.com/kyoungjunpark/VidGuard-R1) |
| [FakeXplain: AI-Generated Image Detection via Human-Aligned Grounded Reasoning](https://openreview.net/pdf?id=UcpTOa8OnG) | ICLR 2026 | `[I]` | Grounded Reasoning, Human-annotated Dataset | N/A |
| [Align, Don't Blend: Orthogonal Supervision Disentanglement As the Key to Generalizable AI-Generated Image Detection](https://arxiv.org/abs/2512.06746) | Arxiv 2026 | `[I]` | Decoupling (Semantic & Pixel), AIGI-Now Dataset | N/A |
| [Locate-Then-Examine: Grounded Region Reasoning Improves Detection of AI-Generated Images](https://openaccess.thecvf.com/content/CVPR2026/papers/Ji_Locate-Then-Examine_Grounded_Region_Reasoning_Improves_Detection_of_AI-Generated_Images_CVPR_2026_paper.pdf) | CVPR 2026 | `[I]` | Thinking with Images, MagniFake Dataset | N/A |
| [AgentFoX: LLM Agent-Guided Fusion with eXplainability for AI-Generated Image Detection](https://arxiv.org/pdf/2603.23115) | Arxiv 2026 | `[I]` | Agentic framework | [Github](https://github.com/suncore946/AgentFoX) |
| [EvoGuard: An Extensible Agentic RL-based Framework for Practical and Evolving AI-Generated Image Detection](https://arxiv.org/pdf/2603.17343) | Arxiv 2026 | `[I]` | Agentic Framework, Method Ensembling | N/A |
| [VIGIL: Part-Grounded Structured Reasoning for Generalizable Deepfake Detection](https://arxiv.org/pdf/2603.21526) | Arxiv 2026 | `[I]` | Part-centric Forensic, OmniFake Dataset | [Project](https://vigil.best/) |
| [GenVideoLens: Where LVLMs Fall Short in AI-Generated Video Detection?](https://arxiv.org/pdf/2603.18625) | Arxiv 2026 | `[V]` | GenVideoLens benchmark | N/A |
| [Semantic Visual Anomaly Detection and Reasoning in AI-Generated Images](https://arxiv.org/pdf/2510.10231) | ICLR 2026 | `[I]` | Semantic Anomaly Reasoning, AnomReason Dataset | N/A |
| [FAKE-HR1: RETHINKING REASONING OF VISION LANGUAGE MODEL FOR SYNTHETIC IMAGE DETECTION](https://doi.org/10.1109/ICASSP55912.2026.11462736) · [arXiv](https://arxiv.org/pdf/2602.10042v1) | ICASSP 2026 | `[I]` | Hybrid-Reasoning, Dual-mode Dataset | N/A |
| [BusterX: MLLM-Powered AI-Generated Video Forgery Detection and Explanation](https://www.alphaxiv.org/pdf/2505.12620) | [NeurIPS 2026](https://neurips.cc/virtual/2026/poster/151123) | `[V]` | GenBuster-200K Dataset, Cold Start + RL Training | [Github](https://github.com/l8cv/BusterX) |
| [REVEAL: Reasoning-enhanced Forensic Evidence Analysis for Explainable AI-generated Image Detection](https://arxiv.org/pdf/2511.23158) | ECCV 2026 | `[I]` | Chain-of-Evidence, Expert-grounded RL | N/A |
| [MIRAGE: Towards AI-Generated Image Detection in the Wild](https://arxiv.org/pdf/2508.13223) | Arxiv 2025 | `[I]` | Human Curation Dataset, Heuristic-to-Analytic Reasoning | [GitHub](https://github.com/och-alibaba/mirage) |
| [BusterX++: Towards Unified Cross-Modal AI-Generated Content Detection and Explanation with MLLM](https://www.alphaxiv.org/pdf/2507.14632) | Arxiv 2025 | `[M]` | RL Post-training, Cross-Modal, Thinking Reward Mechanism | [Github](https://github.com/l8cv/BusterX) |
| [Spot the Fake: Large Multimodal Model-Based Synthetic Image Detection with Artifact Explanation](https://arxiv.org/pdf/2503.14905) | NeurIPS 2025 | `[I]` | FakeClue Dataset, Fine-grained Artifact Clues, Artifact Explanation | [GitHub](https://github.com/opendatalab/FakeVLM) |
| [AIGI-Holmes: Towards Explainable and Generalizable AI-Generated Image Detection via Multimodal Large Language Models](https://arxiv.org/pdf/2507.02664) | ICCV 2025 | `[I]` | Holmes-Set, Multi-Expert Jury, 3-Stage Training Pipeline | [Github](https://github.com/wyczzy/AIGI-Holmes) |
| [LEGION: Learning to Ground and Explain for Synthetic Image Detection](https://arxiv.org/pdf/2503.15264) | ICCV 2025 | `[I]` | SynthScars Dataset, Defender & Controller, Image Refinement | [GitHub](https://github.com/opendatalab/LEGION) |
| [Seeing Before Reasoning: A Unified Framework for Generalizable and Explainable Fake Image Detection](https://arxiv.org/pdf/2509.25502) | Arxiv 2025 | `[I]` | Perception & Reasoning, ExplainFake-Bench | N/A |
| [SIDA: Social Media Image Deepfake Detection, Localization, and Explanation](https://arxiv.org/pdf/2412.04292) | CVPR 2025 | `[I]` | SID-Set, Mask Prediction, Social Media Context | [Github](https://github.com/hzlsaber/SIDA) |
| [FakeShield: Explainable Image Forgery Detection and Localization via Multi-modal Large Language Models](https://arxiv.org/pdf/2410.02761) | ICLR 2025 | `[I]` | Explainable IFDL, Domain Tag-guided, Multi-modal Localization | [GitHub](https://github.com/zhipeixu/FakeShield) |


### Classification-Based
*This category includes supervised learning approaches that train neural networks (CNNs, ViTs, VFMs, etc.) specifically to classify authentic vs. AI-generated content. They usually focus on robustness, generalization, and feature extraction. It is organized into six subcategories: Supervised General Detectors, Video Spatiotemporal Modeling, Training-Free / Zero-Shot, Frequency-Domain & Low-Level Artifacts, Continual & Incremental Learning, and Related & Other.*

#### Supervised General Detectors
*Trainable classifiers and backbones (CNNs, ViTs, vision foundation models, CLIP-based adapters, few-shot and prompt-based methods) for general-purpose detection.*

| Title | Venue & Year | Modality | Highlights/Keywords | Code |
| --- | --- | --- | --- | --- |
| [Less Supervision, Better Generalization: Weakly Supervised Fake Region Localization in Diffusion-Edited Images](https://arxiv.org/abs/2609.36882) | NeurIPS 2026 | `[I]` | ReGFLoW, First Weakly Supervised Diffusion-Edit Localization, Image-Level Labels Only, Diffusion Reconstruction Error as Dense Guidance, Artifact-Centric MIL | N/A |
| [EIB-Net: Entropy-Guided Information Bottleneck for Generalizable AI-Generated Image Detection](https://arxiv.org/abs/2609.29064) | ICME 2026 | `[I]` | Image Entropy (IE) Metric, Lowest-Entropy Patch Selection (EGPL), Variational Information Bottleneck, Local Texture Fidelity Cue, 2% Training Data SOTA, Backbone-Agnostic | N/A |
| [Unifying Semantic Priors and High-Frequency Traces: Enhancing V-JEPA with Mixture-of-Experts for Robust Synthetic Image Forensics](https://arxiv.org/abs/2609.16778) | ECCV 2026 Workshop | `[I]` | MoE-JEPA, V-JEPA 2 World-Model Prior, Residual Mixture-of-Experts, Noise-Stream High-Frequency Branch, Gated Attention MIL, SID-Set SOTA | [GitHub](https://github.com/ALCOR-Lab-DIAG/MoE-JEPA) |
| [From Detection to Localization: A Unified Forensics Framework for Fully Synthetic and Tampered Images](https://arxiv.org/abs/2609.02640) | ACM MM 2026 Workshop | `[I]` | Unified Three-Class Framework (Real / Fully Generated / Tampered), Segmentation Branch for Pixel-Level Localization | [GitHub](https://github.com/anngal01/From-Detection-to-Localization-A-Unified-Forensics-Framework-for-Fully-Synthetic-and-Tampered-Images) |
| [Hierarchical Channel Stacking: A Structured Decision Framework for AI-Generated Image Detection](https://arxiv.org/abs/2608.26648) | ICANN 2026 | `[I]` | Hierarchical CNN Activations, Per-channel Level-1 Classifiers, GAN/Diffusion Stage-level Analysis | N/A |
| [LoRC: Detecting AI-Generated Images via Low-Rank Collapse in Semantic Residuals](https://arxiv.org/abs/2608.20882) | ECCV 2026 (Spotlight) | `[I]` | Low-Rank Collapse Signature, Semantic-Residual Decoupling, Cross-model Generalization | N/A |
| [Harnessing CLIP and DINO: An Uncertainty-Aware Cascaded Fusion Network for Generalizable Deepfake Image Detection](https://arxiv.org/abs/2609.07670) | Arxiv 2026 | `[I]` | UCF-Net, CLIP Semantic + DINO Structural Priors, Layer-wise Expert Aggregation, Entropy-based Uncertainty Fusion, 4M-image Unified Benchmark, Cross-generator Evaluation | [GitHub](https://github.com/XavierJiezou/UCF-Net) |
| [GAP-SAM: A Global Artifact Prior for Generalizable AI-Generated Image Manipulation Localization](https://arxiv.org/abs/2608.20929) | Arxiv 2026 | `[I]` | Global Artifact Token, SAM3 FiLM Injection, Boundary Adhesion Analysis | N/A |
| [Understanding Why Foundation Models Work for Diffusion-Generated Image Detection](https://arxiv.org/abs/2608.12155) | Arxiv 2026 | `[I]` | Interpretability Analysis, DDIM Inversion, Low-to-Mid Frequency Distributional Discrepancy | N/A |
| [PatchHead: Learning Spatial Patch Evidence for Generalizable AI-Generated Image Detection](https://arxiv.org/abs/2608.09223) | Arxiv 2026 | `[I]` | DINO Patch Tokens, 2D Spatial Aggregation, LoRA Adapters | N/A |
| [GlobalForge: Towards Robust AI-Generated Image Detection](https://arxiv.org/abs/2607.14684) | Arxiv 2026 | `[I]` | Global Structural Reasoning, Local Information Bottleneck, RealDeg-Bench | [Code](https://anonymous.4open.science/r/GlobalForge-BE0F/) |
| [Fleet: Few Shots Lead Effective AI-generated Image Detection](https://arxiv.org/abs/2606.31082) | ICML 2026 | `[I]` | Few-shot Adaptation, Routing Correction, Treasure Benchmark | [GitHub](https://github.com/ICTMCG/Fleet) |
| [HydraPrompt: An Adaptive and Asymmetric Framework of Vision-Language Models for Synthetic Image Detection](https://arxiv.org/pdf/2605.26421) | ACM MM 2026 | `[I]` | Asymmetric Prompting, Dynamic Decision Boundary | N/A |
| [Video as Natural Augmentation: Towards Unified AI-Generated Image and Video Detection](https://arxiv.org/pdf/2605.21977) | Arxiv 2026 | `[M]` | Unified Image/Video Detection, Cross-Modal Contrastive Learning | N/A |
| [PGC: Peak-Guided Calibration for Generalizable AI-Generated Image Detection](https://arxiv.org/pdf/2605.21207) | ICML 2026 | `[I]` | Peak-Guided Calibration, CommGen15 Dataset | [GitHub](https://github.com/xiaoyu6868/PGC) |
| [Reduce the Artifacts Bias for More Generalizable AI-Generated Image Detection](https://arxiv.org/pdf/2605.14486) | Arxiv 2026 | `[I]` | Bias-free Training | [GitHub](https://github.com/liyih/SEF_AIGC_detection) |
| [Zooming In on Fakes: A Novel Dataset for Localized AI-Generated Image Detection with Forgery Amplification Approach](https://arxiv.org/abs/2504.11922) | AAAI 2026 | `[I]` | Localized AIGC Detection, Forgery Amplification, Scene-aware Local Forgery | [GitHub](https://github.com/clpbc/BR-Gen) |
| [MIRROR: Manifold Ideal Reference ReconstructOR for AI-Generated Image Detection](https://arxiv.org/pdf/2602.02222) | [NeurIPS 2026](https://neurips.cc/virtual/2026/poster/149292) | `[I]` | Manifold Reconstruction, Memory Bank, Human-AIGI Benchmark | [GitHub](https://github.com/349793927/MIRROR) |
| [No Pixel Left Behind: A Detail-Preserving Architecture for Robust High-Resolution AI-Generated Image Detection](https://arxiv.org/pdf/2508.17346) | ICLR 2026 | `[I]` | Detail-preserving dual-path architecture, Multi-task learning, HiRes-50K benchmark | N/A |
| [All Patches Matter, More Patches Better: Enhance AI-Generated Image Detection via Panoptic Patch Learning](https://arxiv.org/pdf/2504.01396) | ICLR 2026 | `[I]` | Random Patch Replacement, Patch-wise Contrastive Learning | N/A |
| [OmniAID: Decoupling Semantics and Artifacts for Universal AI-Generated Image Detection in the Wild](https://proceedings.mlr.press/v306/guo26ag.html) | ICML 2026 | `[I]` | Mixture-of-Experts, Semantic-Artifact Decoupling, Mirage Dataset | [GitHub](https://github.com/yunncheng/OmniAID) |
| [DINO-Detect: A Simple yet Effective Framework for Blur-Robust AI-Generated Image Detection](https://arxiv.org/pdf/2511.12511) | Arxiv 2025 | `[I]` | Blur Robustness, Knowledge Distillation, DINOv3 | [Github](https://github.com/JiaLiangShen/Dino-Detect-for-blur-robust-AIGC-Detection) |
| [Orthogonal Subspace Decomposition for Generalizable AI-Generated Image Detection](https://proceedings.mlr.press/v267/yan25b.html) | ICML 2025 (Oral) | `[I]` | SVD Orthogonal Subspace, Asymmetry Phenomenon, Parameter-efficient Fine-tuning | [GitHub](https://github.com/YZY-stack/Effort-AIGI-Detection) |
| [A Bias-Free Training Paradigm for More General AI-generated Image Detection](https://arxiv.org/pdf/2412.17671) | CVPR 2025 | `[I]` | Bias-Free, Semantic Alignment, Stable Diffusion Self-conditioning | [Github](https://github.com/grip-unina/B-Free) |
| [Forensics Adapter: Adapting CLIP for Generalizable Face Forgery Detection](https://arxiv.org/pdf/2411.19715) | CVPR 2025 | `[I]` | CLIP, Blending Boundaries, Forgery-aware Prompt Learning | [Github](https://github.com/OUC-VAS/ForensicsAdapter) |
| [Exploring Unbiased Deepfake Detection via Token-Level Shuffling and Mixing](https://arxiv.org/pdf/2501.04376) | AAAI 2025 | `[I]` | Token-Level Shuffling, Contrastive Loss, Bias Mitigation | N/A |
| [FakeFormer: Efficient Vulnerability-Driven Transformers for Generalisable Deepfake Detection](https://arxiv.org/pdf/2410.21964) | Arxiv 2024 | `[I]` | Vulnerability-driven, Local Attention (L2-Att), Vision Transformer | [GitHub](https://github.com/10Ring/FakeFormer) |

#### Video Spatiotemporal Modeling
*Methods that exploit temporal inconsistencies, motion patterns, and spatiotemporal artifacts in AI-generated videos.*

| Title | Venue & Year | Modality | Highlights/Keywords | Code |
| --- | --- | --- | --- | --- |
| [Temporal Slice Learning for AI-Generated Video Detection with 400$\times$ Fewer FLOPs](https://arxiv.org/abs/2610.35148) | NeurIPS 2026 | `[V]` | TSC-Net, Temporal Slice Representation, Frequency-Aware Slice Consistency Learning, Task-Driven Slice Localization, Lightweight Transformer (1.7M Params), 400$\times$ Fewer FLOPs / 3.6$\times$ Faster Inference, GenVideo & AI-Artist Benchmark | N/A |
| [Mind the Rift: Cross-Scale Coupling Mismatch for AI-Generated Video Detection](https://arxiv.org/abs/2609.00742) | ACM MM 2026 | `[V]` | Cross-Scale Coupling Mismatch, Macro Temporal Dynamics vs. Pixel-Level Residuals, Persistent Homology, Encoder-Agnostic | [GitHub](https://github.com/Litsay/RIFT) |
| [MotionPhys: Detecting AI-Generated Videos via Physical Consistency of Optical-Flow Trajectories](https://arxiv.org/abs/2608.20770) | Arxiv 2026 | `[V]` | Physical Motion Consistency, Sparse Optical-Flow Trajectories, Multi-scale Geometric Evolution | N/A |
| [Rethinking the Readout: Unlocking Video Backbones for AI-Generated Video Detection](https://arxiv.org/abs/2607.15321) | [NeurIPS 2026](https://neurips.cc/virtual/2026/poster/149274) | `[V]` | V-PVP Readout, Patch Velocity Profiling, Frozen Video Backbones | [Code](https://anonymous.4open.science/r/PVP-81B3/) |
| [Dataset Biases and Shortcut Learning in Motion-Based AI-Generated Video Detection](https://arxiv.org/abs/2607.00948) | Arxiv 2026 | `[V]` | Motion Bias Analysis, Preprocessing/Sampling Bias, Frequency-based Comparison | N/A |
| [G2VD: Generalizable AI-Generated Video Detection via Counterfactual Intervention and Causal Disentanglement](https://arxiv.org/abs/2607.04607) | Arxiv 2026 | `[V]` | Counterfactual Intervention, Causal Disentanglement, Cross-domain Generalization | Not publicly accessible |
| [ReConFuse: Reconstruction-Error Guided Semantic Fusion for AI-Generated Video Detection](https://arxiv.org/pdf/2606.04706) | Arxiv 2026 | `[V]` | Reconstruction Error, Semantic Fusion, Spatial-Temporal Artifacts | N/A |
| [Detecting AI-Generated Videos with Spiking Neural Networks](https://arxiv.org/pdf/2605.05895) | Arxiv 2026 | `[V]` | Spiking Neural Networks, Temporal Artifact | N/A |
| [CMTA: Leveraging Cross-Modal Temporal Artifacts for Generalizable AI-Generated Video Detection](https://arxiv.org/pdf/2605.00630) | Arxiv 2026 | `[V]` | Cross-Modal Temporal Artifacts, Video Detection | N/A |
| [Preserving Forgery Artifacts: AI-Generated Video Detection at Native Scale](https://openreview.net/pdf?id=XD43lfRCg6) | ICLR 2026 | `[V]` | Native scale video processing, Massive realistic video dataset, Preserves subtle generation artifacts | N/A |
| [DeMamba: AI-Generated Video Detection on Million-Scale GenVideo Benchmark](https://doi.org/10.1007/s11432-024-4894-0) · [arXiv](https://arxiv.org/pdf/2405.19707) | Science China Information Sciences 2026 | `[V]` | Mamba, State Space Model, Long-range Spatiotemporal Inconsistency | [GitHub](https://github.com/chenhaoxing/DeMamba) |
| [Seeing What Matters: Generalizable AI-generated Video Detection with Forensic-Oriented Augmentation](https://arxiv.org/pdf/2506.16802) | NeurIPS 2025 | `[V]` | Wavelet-band Augmentation, Forensic Frequency Artifacts, Single-generator Generalization | [GitHub](https://github.com/grip-unina/WaveRep-SyntheticVideoDetection) |
| [AI-Generated Video Detection via Perceptual Straightening](https://arxiv.org/pdf/2507.00583) | NeurIPS 2025 | `[V]` | Perceptual Straightening, DINOv2, Temporal Curvature | [GitHub](https://github.com/ChristianInterno/ReStraV) |
| [Physics-Driven Spatiotemporal Modeling for AI-Generated Video Detection](https://arxiv.org/pdf/2510.08073) | NeurIPS 2025 | `[V]` | Normalized Spatiotemporal Gradient (NSG), Maximum Mean Discrepancy (MMD) | [Github](https://github.com/ZSHsh98/NSG-VD) |
| [Towards a Universal Synthetic Video Detector: From Face or Background Manipulations to Fully AI-Generated Content](https://arxiv.org/pdf/2412.12278) | CVPR 2025 | `[V]` | SigLIP-So400M, Attention-Diversity Loss, Full-frame Manipulations | N/A |
| [DIP: Diffusion Learning of Inconsistency Pattern for General DeepFake Detection](https://arxiv.org/pdf/2410.23663) | TMM 2025 | `[V]` | Direction-aware Attention, SpatioTemporal Invariant Loss | N/A |

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
| [Structured Local Differential Modeling for AI-Generated Image Detection](https://arxiv.org/abs/2608.12811) | Arxiv 2026 | `[I]` | RippleNet, Local Differential Signals, Low-SNR Forgery Traces | N/A |
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
| [WildAIGC-Bench: Can AI Image Detectors Handle the Wild? A Benchmark of Generated and Edited Images in Online Circulation](https://www.alphaxiv.org/pdf/2610.28087) | arXiv 2026 | `[I]` | [Benchmark] In-the-wild evaluation on generated and edited images circulating online | [GitHub](https://github.com/YuZijian/WildAIGC-Bench) |
| [DF26: We Cannot Tell Fake From Real Anymore](https://arxiv.org/abs/2609.07369) | Arxiv 2026 | `[V]` | [Benchmark] 2,691 Public-Speaking Videos, 7 Modern T2V/I2V Models, Human & SOTA Detectors Near Chance, Distribution-Shift Robustness | N/A |
| [APT: Anchor-aligned Perturbations for Tamper Localization in Fully Regenerated Images](https://arxiv.org/abs/2608.30656) | ECCV 2026 | `[I]` | [Proactive Forensics] Semi-Fragile Latent Perturbation, Fully Regenerated (Inpainting) Setting, Anchor-Direction Alignment | N/A |
| [Training-Free Reconstruction-Based AI-Generated Image Detectors Are Inherently Vulnerable to Adversarial Examples](https://arxiv.org/abs/2608.16646) | ECCV 2026 Workshop | `[I]` | [Robustness Analysis] Reconstruction-based Detector Attacks, Transferable Adversarial Examples, Real-world Degradations | N/A |
| [Can We Defend Against AI-Generated Video Attacks on Real-World Crisis Events? A Systematic Evaluation of Detectors, Generators and Social Dissemination](https://arxiv.org/abs/2608.14391) | Arxiv 2026 | `[V]` | [Evaluation] RA-Bench, Crisis Event Videos, Detector Generalization, Social Dissemination | N/A |
| [When Seeing Is Not Believing -- A Benchmark for Search-Grounded Video Misinformation Detection](https://aclanthology.org/2026.findings-emnlp.763/) | Findings of EMNLP 2026 | `[V]` | Search-Grounded Verification, EVID-Bench, Evidence-Dependent Manipulation | N/A |
| [Robust ASIC-Based Image Authentication Using Reed-Solomon LSB Watermarking](https://github.com/Agnuxo1/Secure_image_generation_with_ASIC_signature) | Preprint 2026 | `[I]` | ASIC PoW, Hardware-bound Provenance, Reed-Solomon Watermarking | [GitHub](https://github.com/Agnuxo1/Secure_image_generation_with_ASIC_signature) |

⬆ [Back to Top](#contents)
