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

- [鹿晗音乐节生图被微博AI误判为“AI生成”：平台检测误判引发热议](https://k.sina.com.cn/article_7879776328_1d5abd84806802529s.html?from=ent)

- [周星驰团队多维度系统应对AI克隆侵权事件](https://ent.sina.cn/2026-07-19/detail-iniihzch1188910.d.html?vt=4)

- [微短剧行业观察：短剧流量狂欢背后，AI内容失范与版权维权破局](https://news.cnr.cn/dj/20260730/t20260730_527737301.shtml)

- [马来西亚启动调查：Grok被指生成性侵类Deepfake内容](https://beta.hyper.ai/cn/stories/74ed19530eac52b5bb893618f65e95dc)

- [公安部：多措并举应对“AI换脸”“深度伪造”等新型技术犯罪](https://www.stdaily.com/web/gdxw/2026-07/24/content_553161.html)

- [今日辟谣（2026年8月13日）：罗某利用AI炮制虚假视频吸粉引流，被依法处罚](https://www.gzwxb.gov.cn/context/contextId/216661)

- [AI造谣，该当何罪（天府新视界）](https://focus.scol.com.cn/zgsz/202607/83282192.html)

- [自然灾害频传，中国面临新挑战——AI伪造视频（BBC中文）](https://www.bbc.com/zhongwen/articles/crmrk3p3e3wo/simp)

- [新一代多模态生成模型MiniMax H3发布并开源，0.8元/秒（新京报）](https://www.bjnews.com.cn/detail/1785474644129260.html)

- [告别“脸崩”时代！AI视频生成模型竞赛加速，谁在为技术买单](https://www.tfcaijing.com/article/page/6b4a4542345a552b43627150477338572f77424b70773d3d)

- [融资密集落地，AI视频大模型竞速商业化](http://www.chinasei.com.cn/dtxw/202608/t20260807_88958.html)

- [2026年8月AI视频模型排行榜：图生视频工具该怎么选？](https://www.pixmax.cn/news/post-58.html)

- [国内外知名大模型及应用汇总（2026/08/14）](https://zhuanlan.zhihu.com/p/670574382)

- [Google给AI水印松绑：允许移除可见水印，但保留不可见SynthID水印与C2PA元数据](https://www.tmtpost.com/agent/ai-article/19884)

- [1000亿张图像被打了水印：SynthID如何变成AI内容治理的隐形基建](https://www.v2code.ai/post/synthid-100b-images-ai-watermark-infrastructure)

- [7月“AI魔改”视频治理成果公布：清理违规视频13300余条、处置违规账号30余个](https://xinwen.bjd.com.cn/content/s6a71a086e4b03fa51a827a09.html)

- [欧盟宣布扩大实施《人工智能法》：8月2日起深度伪造等AI生成内容须明确标注](https://www.news.cn/world/20260731/8fa97d0aefa2467fbfa39096050c1378/c.html)

- [金杜律所：欧盟《AI生成内容透明度行为准则》解读及中欧AIGC标识义务比较](https://www.kingandwood.com/content/kwm/jp/zh/insights/latest-thinking/global-ai-governance-from-risk-identification-to-transparency-obligations)

- [一镜成片，随心参考｜字节跳动 Seedance 2.5 正式发布](https://seed.bytedance.com/zh/blog/one-take-creation-flexible-referencing-introducing-seedance-2-5)

- [因为GPT-image-2，整个互联网都变成了巨大的黑暗森林](https://mp.weixin.qq.com/s/zua1k53RovAOk15Juy6q3g)

- [⭐️ 刚刚，阿里官方认领神秘「欢乐马」(HappyHorse)，来自ATH郑波团队](https://weibo.com/8214551477/5286126636237040)

- [改变视频行业的AI，快来了(但有点恐怖) - Bilibili 影视飓风](https://www.bilibili.com/video/BV1A3cczZEf6/?spm_id_from=333.1387.homepage.video_card.click&vd_source=516db97bb15e7a9ee84b3097ee2ff160)

- [蚂蚁安全实验室获CVPR26 AIGC图像检测挑战赛冠军](https://mp.weixin.qq.com/s/xlvP_rkyaLD0Pfp4g3Jwdw)

- [蚂蚁安全实验室夺冠全球人脸防伪检测挑战赛](https://mp.weixin.qq.com/s/ZZMep9ETEavC99N-GyfRBQ)

- [国家网信办印发《人工智能生成合成内容标识办法》](https://www.cac.gov.cn/2025-03/14/c_1743654684782215.htm)

- [网信部门依法查处“剪映”“猫箱”“即梦AI”等生成合成内容标识违法问题网站平台](https://www.cac.gov.cn/2026-04/28/c_1779119736411711.htm)

- [国家网信办印发《人工智能拟人化互动服务管理暂行办法》](https://www.cac.gov.cn/2026-04/10/c_1777558395078289.htm)

---

## Benchmarks & Datasets

> **Modality Legend:** `[I]` Image | `[V]` Video | `[M]` Multi-modal

> **Annotation Type Legend:** 
> `Au`: Authenticity | `Ex`: Explainability | `Lo`: Localization

| Benchmark | Paper | Venue & Year | Modality | Notes | Real Source | Fake Source/Generator | Annotation | Scale | Download |
| :-------- | :---- | :----------- | :------- | :------ | :---------- | :-------------------- | :--------- | :---- | :------- |
| RealHD | [RealHD: A High-Quality Dataset for Robust Detection of State-of-the-Art AI-Generated Images](https://arxiv.org/abs/2602.10546) | Arxiv 2026 | `[I]` | Multi-category, SOTA Generators, 10K+ Prompts, Inpainting Masks | | T2I, Inpainting, Refinement, Face Swapping | `Au`, `Lo` | 730K+ | [RealHD](https://real-hd.github.io) |
| Treasure | [Fleet: Few Shots Lead Effective AI-generated Image Detection](https://arxiv.org/abs/2606.31082) | ICML 2026 | `[I]` | 64 Models, 20 Closed-source Commercial Engines, Few-shot Adaptation | | Diverse architectures & 20 commercial engines | `Au` | 360K | [Treasure](https://github.com/ICTMCG/Fleet) |
| LADBench | [LADBench: A Benchmark for Logical Fault Detection in Images](https://arxiv.org/pdf/2606.17433) | ICDL 2026 | `[I]` | Logical Anomaly Detection, VLM Evaluation, Common Sense Reasoning | | Synthetic images with logical anomalies | `Au` | 1K+ | [LADBench](https://huggingface.co/datasets/SahasraK/LADBench) |
| EVID-Bench | [When Seeing Is Not Believing -- A Benchmark for Search-Grounded Video Misinformation Detection](https://arxiv.org/pdf/2606.04098) | Arxiv 2026 | `[V]` | Search-Grounded Verification, Evidence-Dependent Manipulation | | | `Au` | | [EVID-Bench](https://huggingface.co/datasets/Kirito-Lab/EVID-Bench) |
| CoCoVideo | [CoCoVideo: The High-Quality Commercial-Model-Based Contrastive Benchmark for AI-Generated Video Detection](https://arxiv.org/pdf/2606.00101) | Arxiv 2026 | `[V]` | Commercial AIGC Models, Contrastive Benchmark | | Commercial video generation models | `Au` | | [CoCoVideo](https://github.com/DonoToT/CoCoVideo) |
| FraudBench | [FraudBench: A Multimodal Benchmark for Detecting AI-Generated Fraudulent Refund Evidence](https://arxiv.org/pdf/2605.08820) | Arxiv 2026 | `[M]` |  Fraudulent Refund Detection (ECommerce) | | | `Au` | | [FraudBench](https://huggingface.co/datasets/TristanYan/FraudBench) |
| GPT-Image-2 Wild | [GPT-Image-2 in the Wild: A Twitter Dataset of Self-Reported AI-Generated Images from the First Week of Deployment](https://arxiv.org/pdf/2604.25370) | Arxiv 2026 | `[I]` | GPT-Image-2 | Twitter (real images) | GPT-Image-2 | `Au` | 10K | [GPT-Image-2 Wild](https://www.scam.ai/en/research) |
| Artifact-Bench | [Artifact-Bench: Evaluating MLLMs on Detecting and Assessing the Artifacts of AI-Generated Videos](https://arxiv.org/pdf/2605.18984) | Arxiv 2026 | `[V]` | MLLM Evaluation, Video Artifacts | | | `Au` | | [Artifact-Bench](https://huggingface.co/datasets/DogNeverSleep/Artifact-Bench) |
| CommGen15 | [PGC: Peak-Guided Calibration for Generalizable AI-Generated Image Detection](https://arxiv.org/pdf/2605.21207) | ICML 2026 | `[I]` | 15 Commercial Generative Models | | 15 commercial generators | `Au` | | [CommGen15](https://modelscope.cn/datasets/xiaoyuzhou68/CommGen15) |
| AEGIS-Academic | [AEGIS: A Holistic Benchmark for Evaluating Forensic Analysis of AI-Generated Academic Images](https://arxiv.org/pdf/2604.28177) | Arxiv 2026 | `[I]` | Academic Image Forensics | | | `Au` | | [AEGIS](https://bupt-reasoning-lab.github.io/AEGIS/) |
| SciFigDetect | [SciFigDetect: A Benchmark for AI-Generated Scientific Figure Detection](https://arxiv.org/pdf/2604.08211) | Arxiv 2026 | `[I]` | Scientific Figure Detection | | Nano Banana Pro, GPT-image-1.5 | `Au` | 150K | [SciFigDetect](https://joyce-yoyo.github.io/SciFigDetect/#access) |
| ActivityForensics | [ActivityForensics: A Comprehensive Benchmark for Localizing Manipulated Activity in Videos](https://arxiv.org/pdf/2604.03819) | CVPR 2026 | `[V]` | Action-level AIGC in videos | | | `Au` | 6K | [ActivityForensics](https://activityforensics.github.io/) |
| MintVid | [VideoVeritas: AI-Generated Video Detection via Perception Pretext Reinforcement Learning](https://arxiv.org/pdf/2602.08828) | ICML 2026 | `[V]` | | OpenVid, VFHQ, HDTF, TikTok | Jimeng3.0-Pro, Seedance, Kling2.5-Turbo, Sora2, TikTok, Youtube, etc.  | `Au` | 4K | [MintVid](https://www.modelscope.cn/datasets/EricTanh/MintVid) |
| AIGVDBench | [Your One-Stop Solution for AI-Generated Video Detection](https://arxiv.org/pdf/2601.11035) | CVPR 2026 | `[V]` | | OpenVid-HD | 31 generation models | `Au` | 440k | [AIGVDBench](https://huggingface.co/datasets/AIGVDBench/AIGVDBench) |
| HydraFake | [Veritas: Generalizable Deepfake Detection via Pattern-Aware Reasoning](https://arxiv.org/pdf/2508.21048) | ICLR 2026(Oral) | `[I]` | | FFHQ, VFHQ, CelebAHQ, FF++, etc. | GPT-4o, HailuoAI, ICLight, InfiniteYou, etc. | `Au`, `Ex` | 100K | [HydraFake](https://www.modelscope.cn/datasets/EricTanh/HydraFake) |
| BR-Gen | [Zooming In on Fakes: A Novel Dataset for Localized AI-Generated Image Detection with Forgery Amplification Approach](https://arxiv.org/abs/2504.11922) | AAAI 2026 | `[I]` | |  |  | `Au`, `Lo` | 150K | [BR-Gen](https://github.com/clpbc/BR-Gen) |
| RRDataset | [Bridging the Gap Between Ideal and Real-world Evaluation: Benchmarking AI-Generated Image Detection in Challenging Scenarios](https://arxiv.org/pdf/2509.09172) | ICCV 2025 | `[I]` | Real-World Robustness, Internet Transmission, Re-digitization | | | `Au` | | N/A |
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
> **Modality Legend:** `[I]` Image | `[V]` Video | `[M]` Multi-modal <br>
> **Category Layout:** Top level is split into **MLLM-Based** (MLLM-powered detection) and **Classification-Based** (compact/traditional classifiers). Classification-Based is further organized into six subcategories. When a paper fits multiple subcategories, the priority is: **Training-Free/Zero-Shot > Continual/Incremental > Video Spatiotemporal > Frequency/Low-Level Artifacts > Supervised General**.

### MLLM-Based
*This category focuses on utilizing Multimodal Large Language Models (MLLMs) like GPT-4V, LLaVA, or Qwen-VL to detect AI-generated content. These methods often provide natural language explanations (explainability) alongside binary detection.*

| Title | Venue & Year | Modality | Highlights/Keywords | Code |
| --- | --- | --- | --- | --- |
| [SPARED: Reasoning-Based AI-Generated Image Detection via Adversarially Edited Data](https://arxiv.org/abs/2608.12876) | Arxiv 2026 | `[I]` | Adversarial RL Loop, Diffusion Editor, Free-form Explanation | N/A |
| [VidForensics-M1: Meta-Detection Reinforcement Learning with Verifiable Temporal Grounding for AI-Generated Video Forensics](https://arxiv.org/abs/2608.11201) | Arxiv 2026 | `[V]` | Meta-Detection RL, Verifiable Temporal Grounding, Evidence-Guided Reward Redistribution | N/A |
| [Veritas++: Value-aware On-Policy Distillation for Perception-Enhanced AIGI Detection](https://arxiv.org/abs/2607.27113) | Arxiv 2026 | `[I]` | Value-aware On-Policy Distillation, Perception-Enhanced Reasoning | [GitHub](https://github.com/EricTan7/VeritasPP) |
| [Detecting AI-Generated Video: A Vision-Language Dual-View Survey](https://arxiv.org/abs/2607.10787) | ACL 2026 Findings | `[V]` | [Survey] Vision-Language Dual-View Taxonomy, Factual Fidelity Verification, Cross-modal Consistency | N/A |
| [TranX-Adapter: Bridging Artifacts and Semantics within MLLMs for Robust AI-generated Image Detection](https://arxiv.org/abs/2602.21716) | ICML 2026 | `[I]` | Artifact feature and Semantic feature fusion | [GitHub](https://github.com/DreamMr/TranX-Adapter) |
| [Venus-DeFakerOne: Unified Fake Image Detection & Localization](https://arxiv.org/pdf/2605.14091) | Arxiv 2026 | `[I]` | Unified Detection & Localization, Large-Scale Training | [GitHub](https://github.com/venus-guangjian/Venus-DeFakerOne) |
| [GenShield: Unified Detection and Artifact Correction for AI-Generated Images](https://arxiv.org/pdf/2605.16122) | ICML 2026 | `[I]` | Unified MLLM, Detect & Correct Artifacts | [GitHub](https://github.com/zhipeixu/GenShield) |
| [ReAlign: Generalizable Image Forgery Detection via Reasoning-Aligned Representation](https://arxiv.org/pdf/2605.16080) | Arxiv 2026 | `[I]` | Reasoning-Aligned Representation, Interpretable | N/A |
| [UniGenDet: A Unified Generative-Discriminative Framework for Co-Evolutionary Image Generation and Generated Image Detection](https://arxiv.org/abs/2604.21904v1) | CVPR 2026 | `[I]` | Unified Model, Co-Evolution (Generation & Detection) | [GitHub](https://github.com/Zhangyr2022/UniGenDet) |
| [VideoVeritas: AI-Generated Video Detection via Perception Pretext Reinforcement Learning](https://arxiv.org/pdf/2602.08828) | ICML 2026 | `[V]` | Perception Pretext RL, Fact-based Reasoning, MintVid Dataset | [GitHub](https://github.com/EricTan7/VideoVeritas) |
| [Veritas: Generalizable deepfake detection via pattern-aware reasoning](https://arxiv.org/pdf/2508.21048) | ICLR 2026(Oral) | `[I]` | Pattern-aware Reasoning, HydraFake Dataset | [Github](https://github.com/EricTan7/Veritas) |
| [DF-LLaVA: Unlocking MLLMs for Synthetic Image Detection via Knowledge Injection and Conflict-Driven Self-Reflection](https://arxiv.org/pdf/2509.14957) | Arxiv 2026 | `[I]` | Knowledge Injection, Self-Reflection | N/A |
| [DocShield: Towards AI Document Safety via Evidence-Grounded Agentic Reasoning](https://arxiv.org/pdf/2604.02694) | Arxiv 2026 | `[M]` | Agentic Framework, Document Safety | N/A |
| [VidGuard-R1: AI-Generated Video Detection and Explanation via Reasoning MLLMs and RL](https://arxiv.org/abs/2510.02282) | ICLR 2026 | `[V]` | Multi-stage RL (GRPO), Time Artifacts, Video Detection Dataset | [GitHub](https://github.com/kyoungjunpark/VidGuard-R1) |
| [FakeXplain: AI-Generated Image Detection via Human-Aligned Grounded Reasoning](https://arxiv.org/pdf/2506.07045) | ICLR 2026 | `[I]` | Grounded Reasoning, Human-annotated Dataset | N/A |
| [AlignGemini: Generalizable AI-Generated Image Detection Through Task-Model Alignment](https://arxiv.org/pdf/2512.06746) | Arxiv 2026 | `[I]` | Decoupling (Semantic & Pixel), AIGI-Now Dataset | N/A |
| [Zoom-In to Sort AI-Generated Images Out](https://arxiv.org/pdf/2510.04225) | Arxiv 2026 | `[I]` | Thinking with Images, MagniFake Dataset | N/A |
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
| [FakeScope: Large Multimodal Expert Model for Transparent AI-Generated Image Forensics](https://arxiv.org/pdf/2503.24267) | Arxiv 2025 | `[I]` | FakeChain Dataset, FakeInstruct, Trace Evidence | N/A |
| [AntifakePrompt: Prompt-Tuned Vision-Language Models are Fake Image Detectors](https://arxiv.org/pdf/2310.17419) | Arxiv 2024 | `[I]` | VQA, InstructBLIP, Soft Prompt-tuning, Zero-shot | [GitHub](https://github.com/nctu-eva-lab/AntifakePrompt) |


### Classification-Based
*This category includes supervised learning approaches that train neural networks (CNNs, ViTs, VFMs, etc.) specifically to classify authentic vs. AI-generated content. They usually focus on robustness, generalization, and feature extraction. It is organized into six subcategories: Supervised General Detectors, Video Spatiotemporal Modeling, Training-Free / Zero-Shot, Frequency-Domain & Low-Level Artifacts, Continual & Incremental Learning, and Related & Other.*

#### Supervised General Detectors
*Trainable classifiers and backbones (CNNs, ViTs, vision foundation models, CLIP-based adapters, few-shot and prompt-based methods) for general-purpose detection.*

| Title | Venue & Year | Modality | Highlights/Keywords | Code |
| --- | --- | --- | --- | --- |
| [Understanding Why Foundation Models Work for Diffusion-Generated Image Detection](https://arxiv.org/abs/2608.12155) | Arxiv 2026 | `[I]` | Interpretability Analysis, DDIM Inversion, Low-to-Mid Frequency Distributional Discrepancy | N/A |
| [PatchHead: Learning Spatial Patch Evidence for Generalizable AI-Generated Image Detection](https://arxiv.org/abs/2608.09223) | Arxiv 2026 | `[I]` | DINO Patch Tokens, 2D Spatial Aggregation, LoRA Adapters | N/A |
| [GlobalForge: Towards Robust AI-Generated Image Detection](https://arxiv.org/abs/2607.14684) | Arxiv 2026 | `[I]` | Global Structural Reasoning, Local Information Bottleneck, RealDeg-Bench | [Code](https://anonymous.4open.science/r/GlobalForge-BE0F/) |
| [Fleet: Few Shots Lead Effective AI-generated Image Detection](https://arxiv.org/abs/2606.31082) | ICML 2026 | `[I]` | Few-shot Adaptation, Routing Correction, Treasure Benchmark | [GitHub](https://github.com/ICTMCG/Fleet) |
| [SSAFE: Simple and Strong AI-Generated Image Detection via Frozen Vision Encoders](https://arxiv.org/abs/2606.08634) | Arxiv 2026 | `[I]` | Frozen Vision Encoders, Linear Classifier, RealWorldBench | N/A |
| [HydraPrompt: An Adaptive and Asymmetric Framework of Vision-Language Models for Synthetic Image Detection](https://arxiv.org/pdf/2605.26421) | ACM MM 2026 | `[I]` | Asymmetric Prompting, Dynamic Decision Boundary | N/A |
| [VINA: Video as Natural Augmentation: Towards Unified AI-Generated Image and Video Detection](https://arxiv.org/pdf/2605.21977) | Arxiv 2026 | `[M]` | Unified Image/Video Detection, Cross-Modal Contrastive Learning | N/A |
| [PGC: Peak-Guided Calibration for Generalizable AI-Generated Image Detection](https://arxiv.org/pdf/2605.21207) | ICML 2026 | `[I]` | Peak-Guided Calibration, CommGen15 Dataset | [GitHub](https://github.com/xiaoyu6868/PGC) |
| [Reduce the Artifacts Bias for More Generalizable AI-Generated Image Detection](https://arxiv.org/pdf/2605.14486) | Arxiv 2026 | `[I]` | Bias-free Training | [GitHub](https://github.com/liyih/SEF_AIGC_detection) |
| [Zooming In on Fakes: A Novel Dataset for Localized AI-Generated Image Detection with Forgery Amplification Approach](https://arxiv.org/abs/2504.11922) | AAAI 2026 | `[I]` | Localized AIGC Detection, Forgery Amplification, Scene-aware Local Forgery | [GitHub](https://github.com/clpbc/BR-Gen) |
| [Simplicity Prevails: The Emergence of Generalizable AIGI Detection in Visual Foundation Models](https://arxiv.org/pdf/2602.01738) | Arxiv 2026 | `[I]` | Linear Probe, Vision Foundation Models, Emergent Forensic Capability | N/A |
| [MIRROR: Manifold Ideal Reference ReconstructOR for Generalizable AI-Generated Image Detection](https://arxiv.org/pdf/2602.02222) | Arxiv 2026 | `[I]` | Manifold Reconstruction, Memory Bank, Human-AIGI Benchmark | [GitHub](https://github.com/349793927/MIRROR) |
| [No Pixel Left Behind: A Detail-Preserving Architecture for Robust High-Resolution AI-Generated Image Detection](https://arxiv.org/pdf/2508.17346) | ICLR 2026 | `[I]` | Detail-preserving dual-path architecture, Multi-task learning, HiRes-50K benchmark | N/A |
| [All Patches Matter, More Patches Better: Enhance AI-Generated Image Detection via Panoptic Patch Learning](https://arxiv.org/pdf/2504.01396) | ICLR 2026 | `[I]` | Random Patch Replacement, Patch-wise Contrastive Learning | N/A |
| [OmniAID: Decoupling Semantic and Artifacts for Universal AI-Generated Image Detection in the Wild](https://arxiv.org/pdf/2511.08423) | Arxiv 2025 | `[I]` | Mixture-of-Experts, Semantic-Artifact Decoupling, Mirage Dataset | [GitHub](https://github.com/yunncheng/OmniAID) |
| [DINO-Detect: A Simple yet Effective Framework for Blur-Robust AI-Generated Image Detection](https://arxiv.org/pdf/2511.12511) | Arxiv 2025 | `[I]` | Blur Robustness, Knowledge Distillation, DINOv3 | [Github](https://github.com/JiaLiangShen/Dino-Detect-for-blur-robust-AIGC-Detection) |
| [Orthogonal Subspace Decomposition for Generalizable AI-Generated Image Detection](https://arxiv.org/pdf/2411.15633) | ICML 2025 (Oral) | `[I]` | SVD Orthogonal Subspace, Asymmetry Phenomenon, Parameter-efficient Fine-tuning | [GitHub](https://github.com/zhiyuan-yan/Effort) |
| [A Bias-Free Training Paradigm for More General AI-generated Image Detection](https://arxiv.org/pdf/2412.17671) | CVPR 2025 | `[I]` | Bias-Free, Semantic Alignment, Stable Diffusion Self-conditioning | [Github](https://github.com/grip-unina/B-Free) |
| [Forensics Adapter: Adapting CLIP for Generalizable Face Forgery Detection](https://arxiv.org/pdf/2411.19715) | CVPR 2025 | `[I]` | CLIP, Blending Boundaries, Forgery-aware Prompt Learning | [Github](https://github.com/OUC-VAS/ForensicsAdapter) |
| [Exploring Unbiased Deepfake Detection via Token-Level Shuffling and Mixing](https://arxiv.org/pdf/2501.04376) | AAAI 2025 | `[I]` | Token-Level Shuffling, Contrastive Loss, Bias Mitigation | N/A |
| [FakeFormer: Efficient Vulnerability-Driven Transformers for Generalisable Deepfake Detection](https://arxiv.org/pdf/2410.21964) | Arxiv 2024 | `[I]` | Vulnerability-driven, Local Attention (L2-Att), Vision Transformer | [GitHub](https://github.com/10Ring/FakeFormer) |

#### Video Spatiotemporal Modeling
*Methods that exploit temporal inconsistencies, motion patterns, and spatiotemporal artifacts in AI-generated videos.*

| Title | Venue & Year | Modality | Highlights/Keywords | Code |
| --- | --- | --- | --- | --- |
| [Rethinking the Readout: Unlocking Video Backbones for AI-Generated Video Detection](https://arxiv.org/abs/2607.15321) | Arxiv 2026 | `[V]` | V-PVP Readout, Patch Velocity Profiling, Frozen Video Backbones | [Code](https://anonymous.4open.science/r/PVP-81B3/) |
| [Dataset Biases and Shortcut Learning in Motion-Based AI-Generated Video Detection](https://arxiv.org/abs/2607.00948) | Arxiv 2026 | `[V]` | Motion Bias Analysis, Preprocessing/Sampling Bias, Frequency-based Comparison | N/A |
| [G2VD: Generalizable AI-Generated Video Detection via Counterfactual Intervention and Causal Disentanglement](https://arxiv.org/abs/2607.04607) | Arxiv 2026 | `[V]` | Counterfactual Intervention, Causal Disentanglement, Cross-domain Generalization | [GitHub](https://github.com/dumeng98/G2VD) |
| [ReConFuse: Reconstruction-Error Guided Semantic Fusion for AI-Generated Video Detection](https://arxiv.org/pdf/2606.04706) | Arxiv 2026 | `[V]` | Reconstruction Error, Semantic Fusion, Spatial-Temporal Artifacts | N/A |
| [Detecting AI-Generated Videos with Spiking Neural Networks](https://arxiv.org/pdf/2605.05895) | Arxiv 2026 | `[V]` | Spiking Neural Networks, Temporal Artifact | N/A |
| [CMTA: Leveraging Cross-Modal Temporal Artifacts for Generalizable AI-Generated Video Detection](https://arxiv.org/pdf/2605.00630) | Arxiv 2026 | `[V]` | Cross-Modal Temporal Artifacts, Video Detection | N/A |
| [Preserving Forgery Artifacts: AI-Generated Video Detection at Native Scale](https://openreview.net/pdf?id=XD43lfRCg6) | ICLR 2026 | `[V]` | Native scale video processing, Massive realistic video dataset, Preserves subtle generation artifacts | N/A |
| [Seeing What Matters: Generalizable AI-generated Video Detection with Forensic-Oriented Augmentation](https://arxiv.org/pdf/2506.16802) | NeurIPS 2025 | `[V]` | Wavelet-band Augmentation, Forensic Frequency Artifacts, Single-generator Generalization | [GitHub](https://github.com/grip-unina/WaveRep-SyntheticVideoDetection) |
| [AI-Generated Video Detection via Perceptual Straightening](https://arxiv.org/pdf/2507.00583) | NeurIPS 2025 | `[V]` | Perceptual Straightening, DINOv2, Temporal Curvature | [GitHub](https://github.com/ChristianInterno/ReStraV) |
| [Physics-Driven Spatiotemporal Modeling for AI-Generated Video Detection](https://arxiv.org/pdf/2510.08073) | NeurIPS 2025 | `[V]` | Normalized Spatiotemporal Gradient (NSG), Maximum Mean Discrepancy (MMD) | [Github](https://github.com/ZSHsh98/NSG-VD) |
| [Towards a Universal Synthetic Video Detector: From Face or Background Manipulations to Fully AI-Generated Content](https://arxiv.org/pdf/2412.12278) | CVPR 2025 | `[V]` | SigLIP-So400M, Attention-Diversity Loss, Full-frame Manipulations | N/A |
| [DIP: Diffusion Learning of Inconsistency Pattern for General DeepFake Detection](https://arxiv.org/pdf/2410.23663) | TMM 2025 | `[V]` | Direction-aware Attention, SpatioTemporal Invariant Loss | N/A |
| [DeMamba: AI-Generated Video Detection on Million-Scale GenVideo Benchmark](https://arxiv.org/pdf/2405.19707) | Arxiv 2024 | `[V]` | Mamba, State Space Model, Long-range Spatiotemporal Inconsistency | [GitHub](https://github.com/chenhaoxing/DeMamba) |
| [Distinguish Any Fake Videos: Unleashing the Power of Large-scale Data and Motion Features](https://arxiv.org/pdf/2405.15343) | Arxiv 2024 | `[V]` | GenVidDet, Optical Flow, Dual-Branch 3D Transformer | N/A |

#### Training-Free / Zero-Shot
*Methods that detect AI-generated content without additional training on detection data.*

| Title | Venue & Year | Modality | Highlights/Keywords | Code |
| --- | --- | --- | --- | --- |
| [SPLIT: Training-Free AI-Generated and Partially Edited Video Detection via Spatial Patch-Level Incoherence and Temporal Roughness](https://arxiv.org/abs/2607.02886) | ECCV 2026 | `[V]` | Training-free, Patch-level Incoherence, Temporal Roughness, Ultra-low FPR | [GitHub](https://github.com/mldljyh/SPLIT) |
| [Training-free Detection of Generated Videos via Spatial-Temporal Likelihoods](https://arxiv.org/pdf/2603.15026) | CVPR 2026 | `[V]` | Training-free, Zero-shot, Spatial-Temporal Likelihoods, ComGenVid Dataset | [GitHub](https://github.com/OmerBenHayun/STALL) |

#### Frequency-Domain & Low-Level Artifacts
*Methods based on spectral analysis, quantization/upsampling traces, and other low-level generative artifacts.*

| Title | Venue & Year | Modality | Highlights/Keywords | Code |
| --- | --- | --- | --- | --- |
| [Structured Local Differential Modeling for AI-Generated Image Detection](https://arxiv.org/abs/2608.12811) | Arxiv 2026 | `[I]` | RippleNet, Local Differential Signals, Low-SNR Forgery Traces | N/A |
| [Dual Data Alignment Makes AI-Generated Image Detector Easier Generalizable](https://arxiv.org/pdf/2505.14359) | NeurIPS 2025 (Spotlight) | `[I]` | Dual-domain Alignment, Frequency-level Bias, VAE Reconstruction | [GitHub](https://github.com/roy-ch/Dual-Data-Alignment) |
| [D3QE: Learning Discrete Distribution Discrepancy-aware Quantization Error for Autoregressive-Generated Image Detection](https://openaccess.thecvf.com/content/ICCV2025/papers/Zhang_D3QE_Learning_Discrete_Distribution_Discrepancy-aware_Quantization_Error_for_Autoregressive-Generated_Image_ICCV_2025_paper.pdf) | ICCV 2025 | `[I]` | Discrete Distribution Discrepancy-aware Transformer, Vector Quantized Variational AutoEncoder | [Github](https://github.com/Zhangyr2022/D3QE) |
| [Any-Resolution AI-Generated Image Detection by Spectral Learning](https://arxiv.org/pdf/2411.19417) | CVPR 2025 | `[I]` | Spectral Context Attention, Frequency Reconstruction, OOD Detection | [Github](https://github.com/kartyg23/spai) |
| [Frequency-Aware Deepfake Detection: Improving Generalizability through Frequency Space Domain Learning](https://arxiv.org/pdf/2403.07240) | AAAI 2024 | `[I]` | Frequency Domain, FFT, Frequency Conv Layer (FCL), Lightweight | [GitHub](https://github.com/chuangchuangtan/FreqNet-DeepfakeDetection) |
| [Rethinking the Up-Sampling Operations in CNN-based Generative Network](https://arxiv.org/pdf/2312.10461) | CVPR 2024 | `[I]` | Neighboring Pixel Relationships, Generalized Structural Artifacts | [Github](https://github.com/chuangchuangtan/NPR-DeepfakeDetection) |

#### Continual & Incremental Learning
*Methods that keep adapting detectors to evolving generators without catastrophic forgetting.*

| Title | Venue & Year | Modality | Highlights/Keywords | Code |
| --- | --- | --- | --- | --- |
| [Automated In-the-Wild Data Collection for Continual AI Generated Image Detection](https://arxiv.org/pdf/2605.02567) | Arxiv 2026 | `[I]` | Continual Learning, Continual Data Collection | [GitHub](https://mever-team.github.io/WildFC/) |
| [IncreFA: Breaking the Static Wall of Generative Model Attribution](https://arxiv.org/pdf/2604.17736) | Arxiv 2026 | `[I]` | Incremental Learning, Generative Model Attribution | [GitHub](https://github.com/Ant0ny44/IncreFA) |
| [SAIDO: Generalizable Detection of AI-Generated Images via Scene-Aware and Importance-Guided Dynamic Optimization in Continual Learning](https://arxiv.org/pdf/2512.00539) | CVPR 2026 | `[I]` | Scene-aware optimization, Continual learning | [GitHub](https://github.com/edu-yinzhaoxia/SAIDO-CVPR2026) |
| [Generalizable and Adaptive Continual Learning Framework for AI-generated Image Detection](https://arxiv.org/pdf/2601.05580) | TMM 2026 | `[I]` | Continual Learning, Kronecker-Factored Approximate Curvature | N/A |

#### Related & Other
*Papers related to AI-generated content safety (e.g., provenance/watermarking, misinformation verification) that do not fit the subcategories above.*

| Title | Venue & Year | Modality | Highlights/Keywords | Code |
| --- | --- | --- | --- | --- |
| [Can We Defend Against AI-Generated Video Attacks on Real-World Crisis Events? A Systematic Evaluation of Detectors, Generators and Social Dissemination](https://arxiv.org/abs/2608.14391) | Arxiv 2026 | `[V]` | [Evaluation] RA-Bench, Crisis Event Videos, Detector Generalization, Social Dissemination | N/A |
| [When Seeing Is Not Believing -- A Benchmark for Search-Grounded Video Misinformation Detection](https://arxiv.org/pdf/2606.04098) | Arxiv 2026 | `[V]` | Search-Grounded Verification, EVID-Bench, Evidence-Dependent Manipulation | N/A |
| [Robust ASIC-Based Image Authentication Using Reed-Solomon LSB Watermarking](https://github.com/Agnuxo1/Secure_image_generation_with_ASIC_signature) | Preprint 2026 | `[I]` | ASIC PoW, Hardware-bound Provenance, Reed-Solomon Watermarking | [GitHub](https://github.com/Agnuxo1/Secure_image_generation_with_ASIC_signature) |

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
