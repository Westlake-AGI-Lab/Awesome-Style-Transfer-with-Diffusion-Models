<!-- <div align="center">
<h2> Awesome Style Transfer with Diffusion Models </h2> 
</div> -->
# 🥳Awesome Style Transfer with Diffusion Models [![Awesome](https://awesome.re/badge.svg)](https://awesome.re) 

# 🤗 Introduction
- This repository contains a curated list of **Style Transfer with Diffusion Models**. The resources are organized into two main categories: Image Synthesis and Video Synthesis. 

- We welcome any contributions and suggestions to our repository or the addition of your own work. Feel free to make a pull request or leave your comments!!

# 📋 Contents
- [🤗 Introduction](#-introduction)
- [📋 Contents](#-contents)
- [🤔 Perspectives](#-perspectives)
- [📍 Image Synthesis](#-image-synthesis)
  - [Fundation & Application Models](#foundation--application-models)
  - [Image-Encoder Based](#image-encoder-based)
  - [Swap Features In Attention Layer](#swap-features-in-attention-layer)
  - [Optimization-Based Methods](#optimization-based-methods)
  - [LoRA-Based](#lora-based-methods)
- [📍 Video Synthesis](#-video-synthesis)
- [📍 3D Generation](#-3d-generation)
- [📍 Style Dataset](#-style-dataset)
- [📍 Related Research and Surveys](#-related-research-and-surveys)

# 🤔 Perspectives
*A personal view from the maintainers, September 2026.*

Style is vague and hard to define. Seen from one angle, style is also a kind of semantics, and the difficulty of this task lies in separating out the many different kinds of semantics. The diversity of style itself then makes that separation and disentanglement harder.

Style transfer is also more of an application, and every user has their own view of it.

We reorganized the paper taxonomy to focus more on how a method encodes the style image. For example, an image encoder is a feed-forward any-style method, while a LoRA-based method applies to a single style.

# 📍 Image Synthesis

In the context of Image Style Transfer, the techniques can be categorized into two primary types: text-driven style transfer and image-driven style transfer and the techniques are organized by the mechanism that carries the style: image encoders and adapters, attention feature swapping, LoRA, and optimization-based methods.

## Foundation & Application Models
| Title | Github | Pub. & Date |
| :--- | :---: | :---: |
|[FLUX.1 Kontext: Flow Matching for In-Context Image Generation and Editing in Latent Space](https://arxiv.org/abs/2506.15742)|[![Star](https://img.shields.io/github/stars/black-forest-labs/flux.svg?style=social&label=Star)](https://github.com/black-forest-labs/flux)|Jun., 2025|
|[Qwen-Image Technical Report](https://arxiv.org/abs/2508.02324)|[![Star](https://img.shields.io/github/stars/QwenLM/Qwen-Image.svg?style=social&label=Star)](https://github.com/QwenLM/Qwen-Image)|Aug., 2025|
|[Skywork UniPic: Unified Autoregressive Modeling for Visual Understanding and Generation](https://www.arxiv.org/abs/2508.03320)|[![Star](https://img.shields.io/github/stars/SkyworkAI/UniPic.svg?style=social&label=Star)](https://github.com/SkyworkAI/UniPic)|Aug., 2025|
|[Unified Customized Generation by Disentangled Reward Modeling](https://openaccess.thecvf.com/content/CVPR2026/papers/Wu_Unified_Customized_Generation_by_Disentangled_Reward_Modeling_CVPR_2026_paper.pdf)|[![Star](https://img.shields.io/github/stars/bytedance/USO.svg?style=social&label=Star)](https://github.com/bytedance/USO)|CVPR 2026|


## Image-Encoder Based
| Title | Github | Pub. & Date |
| :--- | :---: | :---: |
|[IP-Adapter: Text Compatible Image Prompt Adapter for Text-to-Image Diffusion Models](https://arxiv.org/abs/2308.06721)|[![Star](https://img.shields.io/github/stars/tencent-ailab/IP-Adapter.svg?style=social&label=Star)](https://github.com/tencent-ailab/IP-Adapter)|Aug., 2023|
|[StyleAdapter: A Unified Stylized Image Generation Model](https://arxiv.org/abs/2309.01770)|-|Sep., 2023|
|[ArtAdapter: Text-to-Image Style Transfer using Multi-Level Style Encoder and Explicit Adaptation](https://arxiv.org/abs/2312.02109)|[![Star](https://img.shields.io/github/stars/cardinalblue/ArtAdapter.svg?style=social&label=Star)](https://github.com/cardinalblue/ArtAdapter)|CVPR 2024|
|[HiCAST: Highly Customized Arbitrary Style Transfer with Adapter Enhanced Diffusion Models](https://arxiv.org/abs/2401.05870)|[![Star](https://img.shields.io/github/stars/wd1511/HiCAST.svg?style=social&label=Star)](https://github.com/wd1511/HiCAST)|Jan., 2024|
|[DEADiff: An Efficient Stylization Diffusion Model with Disentangled Representations](https://arxiv.org/abs/2403.06951)|[![Star](https://img.shields.io/github/stars/bytedance/DEADiff.svg?style=social&label=Star)](https://github.com/bytedance/DEADiff)|CVPR 2024|
|[InstantStyle: Free Lunch towards Style-Preserving in Text-to-Image Generation](https://arxiv.org/abs/2404.02733)|[![Star](https://img.shields.io/github/stars/instantX-research/InstantStyle.svg?style=social&label=Star)](https://github.com/instantX-research/InstantStyle)|Apr., 2024|
|[StyleMaster: Towards Flexible Stylized Image Generation with Diffusion Models](https://arxiv.org/abs/2405.15287v1)|-|May, 2024|
|[InstantStyle-Plus: Style Transfer with Content-Preserving in Text-to-Image Generation](https://arxiv.org/abs/2407.00788)|[![Star](https://img.shields.io/github/stars/instantX-research/InstantStyle-Plus.svg?style=social&label=Star)](https://github.com/instantX-research/InstantStyle-Plus)|Jun., 2024|
|[StyleShot: A Snapshot on Any Style](https://arxiv.org/abs/2407.01414)|[![Star](https://img.shields.io/github/stars/open-mmlab/StyleShot.svg?style=social&label=Star)](https://github.com/open-mmlab/StyleShot)|Jul., 2024|
|[D2Styler: Advancing Arbitrary Style Transfer with Discrete Diffusion Methods](https://arxiv.org/abs/2408.03558)|[![Star](https://img.shields.io/github/stars/Onkarsus13/D2Styler.svg?style=social&label=Star)](https://github.com/Onkarsus13/D2Styler)|ICPR 2024|
|[CSGO: Content-Style Composition in Text-to-Image Generation](https://arxiv.org/abs/2408.16766)|[![Star](https://img.shields.io/github/stars/instantX-research/CSGO.svg?style=social&label=Star)](https://github.com/instantX-research/CSGO)|Aug., 2024|
|[StyleTokenizer: Defining Image Style by a Single Instance for Controlling Diffusion Models](https://arxiv.org/abs/2409.02543)|[![Star](https://img.shields.io/github/stars/alipay/style-tokenizer.svg?style=social&label=Star)](https://github.com/alipay/style-tokenizer)|ECCV 2024|
|[StyleStudio: Text-Driven Style Transfer with Selective Control of Style Elements](https://arxiv.org/abs/2412.08503)|[![Star](https://img.shields.io/github/stars/Westlake-AGI-Lab/StyleStudio.svg?style=social&label=Star)](https://github.com/Westlake-AGI-Lab/StyleStudio)|CVPR 2025|
|[EasyRef: Omni-Generalized Group Image Reference for Diffusion Models via Multimodal LLM](https://arxiv.org/abs/2412.09618v1)|-|Dec., 2024|
|[ArtCrafter: Text-Image Aligning Style Transfer via Embedding Reframing](https://arxiv.org/abs/2501.02064)|-|Jan., 2025|
|[Less is More: Masking Elements in Image Condition Features Avoids Content Leakages in Style Transfer Diffusion Models](https://arxiv.org/abs/2502.07466)|[![Star](https://img.shields.io/github/stars/LinLLLL/MaskST.svg?style=social&label=Star)](https://github.com/LinLLLL/MaskST)|ICLR 2025|
|[Free-Lunch Color-Texture Disentanglement for Stylized Image Generation](https://arxiv.org/abs/2503.14275?)|[![Star](https://img.shields.io/github/stars/deepffff/SADis.svg?style=social&label=Star)](https://github.com/deepffff/SADis)|Mar., 2025|
|[OmniStyle: Filtering High Quality Style Transfer Data at Scale](https://arxiv.org/abs/2505.14028)|-|CVPR 2025|
|[Domain Generalizable Portrait Style Transfer](https://arxiv.org/abs/2507.04243)|-|Jul., 2025|
|[CleanStyle: Plug-and-Play Style Conditioning Purification for Text-to-Image Stylization](https://arxiv.org/abs/2602.20721)|[![Star](https://img.shields.io/github/stars/Westlake-AGI-Lab/CleanStyle.svg?style=social&label=Star)](https://github.com/Westlake-AGI-Lab/CleanStyle)|Feb., 2026|
|[MegaStyle: Constructing Diverse and Scalable Style Dataset via Consistent Text-to-Image Style Mapping](https://arxiv.org/abs/2604.08364)|[![Star](https://img.shields.io/github/stars/Tencent/MegaStyle.svg?style=social&label=Star)](https://github.com/Tencent/MegaStyle)|CVPR 2026|
|[StyleBoost: Controlling style-content fusion with SVD for text-driven](https://www.sciencedirect.com/science/article/pii/S0925231225025159)|-|Neurocomputing|
|[Color-Style Disentangled Two-Stream Networks for Universal Tuning-Free Style Transfer](https://www.researchgate.net/profile/Shiwen-Zhang-9/publication/393789188_Color-Style_Disentangled_Two-Stream_Networks_for_Universal_Tuning-Free_Style_Transfer/links/687a15a64f72461c714f3d41/Color-Style-Disentangled-Two-Stream-Networks-for-Universal-Tuning-Free-Style-Transfer.pdf)|-|Jul., 2025|
|[FAST: Flexibly Controllable Arbitrary Style Transfer via Latent Diffusion models](https://dl.acm.org/doi/pdf/10.1145/3748655)|[![Star](https://img.shields.io/github/stars/wd1511/FAST.svg?style=social&label=Star)](https://github.com/wd1511/FAST)|ToMM 2025|
|[Mixture of Style Experts for Diverse Image Stylization](https://openaccess.thecvf.com/content/CVPR2026/papers/Zhu_Mixture_of_Style_Experts_for_Diverse_Image_Stylization_CVPR_2026_paper.pdf)|[![Star](https://img.shields.io/github/stars/HVision-NKU/StyleExpert.svg?style=social&label=Star)](https://github.com/HVision-NKU/StyleExpert)|CVPR 2026|

## Swap Features In Attention Layer
| Title | Github | Pub. & Date |
| :--- | :---: | :---: |
|[Cross-Image Attention for Zero-Shot Appearance Transfer](https://arxiv.org/abs/2311.03335)|[![Star](https://img.shields.io/github/stars/garibida/cross-image-attention.svg?style=social&label=Star)](https://github.com/garibida/cross-image-attention)|SIGGRAPH 2024|
|[Z-STAR: Zero-shot Style Transfer via Attention Rearrangement](https://arxiv.org/abs/2311.16491)|[![Star](https://img.shields.io/github/stars/HolmesShuan/Zero-shot-Style-Transfer-via-Attention-Rearrangement.svg?style=social&label=Star)](https://github.com/HolmesShuan/Zero-shot-Style-Transfer-via-Attention-Rearrangement)|CVPR 2024|
|[Style Aligned Image Generation via Shared Attention](https://arxiv.org/abs/2312.02133)|[![Star](https://img.shields.io/github/stars/google/style-aligned.svg?style=social&label=Star)](https://github.com/google/style-aligned/)|CVPR 2024|
|[Style Injection in Diffusion: A Training-free Approach for Adapting Large-scale Diffusion Models for Style Transfer](https://arxiv.org/abs/2312.09008)|[![Star](https://img.shields.io/github/stars/jiwoogit/StyleID.svg?style=social&label=Star)](https://github.com/jiwoogit/StyleID)|CVPR 2024|
|[Visual Style Prompting with Swapping Self-Attention](https://arxiv.org/abs/2402.12974)|[![Star](https://img.shields.io/github/stars/naver-ai/Visual-Style-Prompting.svg?style=social&label=Star)](https://github.com/naver-ai/Visual-Style-Prompting)|Feb., 2024|
|[Training-free Color-Style Disentanglement for Constrained Text-to-Image Synthesis](https://arxiv.org/abs/2409.02429)|-|Sep., 2024|
|[AttenST: A Training-Free Attention-Driven Style Transfer Framework with Pre-Trained Diffusion Models](https://arxiv.org/abs/2503.07307)|[![Star](https://img.shields.io/github/stars/HuanBor/AttenST.svg?style=social&label=Star)](https://github.com/HuanBor/AttenST)|Mar., 2025|
|[Training-free Stylized Text-to-Image Generation with Fast Inference](https://arxiv.org/abs/2505.19063?)|[![Star](https://img.shields.io/github/stars/maxin-cn/OmniPainter.svg?style=social&label=Star)](https://github.com/maxin-cn/OmniPainter)|May, 2025|
|[SPG: Style-Prompting Guidance for Style-Specific Content Creation](https://arxiv.org/abs/2508.11476)|[![Star](https://img.shields.io/github/stars/Rumbling281441/SPG.svg?style=social&label=Star)](https://github.com/Rumbling281441/SPG)|Aug., 2025|
|[StyleKeeper: Prevent Content Leakage using Negative Visual Query Guidance](https://arxiv.org/abs/2510.06827)|-|Oct., 2025|
|[StyleGuide: Crafting visual style prompting with negative visual query guidance](https://openreview.net/pdf?id=618qfjvSt9)|-|Sep., 2024|
|[STAM: Zero-Shot Style Transfer using Diffusion Model via Attention Modulation](https://openaccess.thecvf.com/content/CVPR2025W/CVEU/papers/Fahim_STAM_Zero-Shot_Style_Transfer_using_Diffusion_Model_via_Attention_Modulation_CVPRW_2025_paper.pdf)|-|CVPR 2025 WorkShop|
|[HAM: A Training-Free Style Transfer Approach via Heterogeneous Attention Modulation for Diffusion Models](https://openaccess.thecvf.com/content/CVPR2026F/papers/He_HAM_A_Training-Free_Style_Transfer_Approach_via_Heterogeneous_Attention_Modulation_CVPRF_2026_paper.pdf)|-|CVPR 2026 Findings|

## Optimization-Based Methods
| Title | Github | Pub. & Date |
| :--- | :---: | :---: |
|[An Image is Worth One Word: Personalizing Text-to-Image Generation using Textual Inversion](https://arxiv.org/abs/2208.01618)|[![Star](https://img.shields.io/github/stars/rinongal/textual_inversion.svg?style=social&label=Star)](https://github.com/rinongal/textual_inversion)|ICLR 2023|
|[DiffStyler: Controllable Dual Diffusion for Text-Driven Image Stylization](https://arxiv.org/abs/2211.10682)|[![Star](https://img.shields.io/github/stars/haha-lisa/Diffstyler.svg?style=social&label=Star)](https://github.com/haha-lisa/Diffstyler)|Nov., 2022|
|[Inversion-Based Style Transfer with Diffusion Models](https://arxiv.org/abs/2211.13203)|[![Star](https://img.shields.io/github/stars/zyxElsa/InST.svg?style=social&label=Star)](https://github.com/zyxElsa/InST)|CVPR 2023|
|[Zero-Shot Contrastive Loss for Text-Guided Diffusion Image Style Transfer](https://arxiv.org/pdf/2303.08622)|-|ICCV 2023|
|[FreeDoM: Training-Free Energy-Guided Conditional Diffusion Model](https://arxiv.org/abs/2303.09833)|[![Star](https://img.shields.io/github/stars/vvictoryuki/FreeDoM.svg?style=social&label=Star)](https://github.com/vvictoryuki/FreeDoM)|ICCV 2023|
|[Null-text Guidance in Diffusion Models is Secretly a Cartoon-style Creator](https://arxiv.org/abs/2305.06710)|[![Star](https://img.shields.io/github/stars/NullTextforCartoon/NullTextforCartoon.svg?style=social&label=Star)](https://github.com/NullTextforCartoon/NullTextforCartoon)|MM 2023|
|[StyleDrop: Text-to-Image Generation in Any Style](https://arxiv.org/abs/2306.00983)|-|NeurIPS 2023|
|[General Image-to-Image Translation with One-Shot Image Guidance](https://arxiv.org/abs/2307.14352)|[![Star](https://img.shields.io/github/stars/CrystalNeuro/visual-concept-translator.svg?style=social&label=Star)](https://github.com/CrystalNeuro/visual-concept-translator)|Jul., 2023|
|[StyleDiffusion: Controllable Disentangled Style Transfer via Diffusion Models](https://arxiv.org/abs/2308.07863)|-|ICCV 2023|
|[DreamStyler: Paint by Style Inversion with Text-to-Image Diffusion Models](https://arxiv.org/abs/2309.06933)|[![Star](https://img.shields.io/github/stars/webtoon/dreamstyler.svg?style=social&label=Star)](https://github.com/webtoon/dreamstyler)|AAAI 2024|
|[ControlStyle: Text-Driven Stylized Image Generation Using Diffusion Priors](https://arxiv.org/abs/2311.05463)|-|MM 2023|
|[An Image is Worth Multiple Words: Multi-attribute Inversion for Constrained Text-to-Image Synthesis](https://arxiv.org/abs/2311.11919)|-|Nov., 2023|
|[ArtBank: Artistic Style Transfer with Pre-trained Diffusion Model and Implicit Style Prompt Bank](https://arxiv.org/abs/2312.06135)|[![Star](https://img.shields.io/github/stars/Jamie-Cheung/ArtBank.svg?style=social&label=Star)](https://github.com/Jamie-Cheung/ArtBank)|AAAI 2024|
|[Towards Highly Realistic Artistic Style Transfer via Stable Diffusion with Step-aware and Layer-aware Prompt](https://arxiv.org/abs/2404.11474)|[![Star](https://img.shields.io/github/stars/Jamie-Cheung/LSAST.svg?style=social&label=Star)](https://github.com/Jamie-Cheung/LSAST)|IJCAI 2024|
|[StyleBooth: Image Style Editing with Multimodal Instruction](https://arxiv.org/abs/2404.12154)|[![Star](https://img.shields.io/github/stars/modelscope/scepter.svg?style=social&label=Star)](https://github.com/modelscope/scepter)|Apr., 2024|
|[VectorPainter: Advanced Stylized Vector Graphics Synthesis Using Stroke-Style Priors](https://arxiv.org/abs/2405.02962)|-|ICME 2025|
|[RB-Modulation: Training-Free Personalization of Diffusion Models using Stochastic Optimal Control](https://arxiv.org/abs/2405.17401)|[![Star](https://img.shields.io/github/stars/google/RB-Modulation.svg?style=social&label=Star)](https://github.com/google/RB-Modulation)|ICLR 2025|
|[Frequency-Controlled Diffusion Model for Versatile Text-Guided Image-to-Image Translation](https://arxiv.org/abs/2407.03006)|-|AAAI 2024|
|[Single Trajectory Distillation for Accelerating Image and Video Style Transfer](https://arxiv.org/abs/2412.18945v1)|-|Dec., 2024|
|[StyleSSP: Sampling StartPoint Enhancement for Training-free Diffusion-based Method for Style Transfer](https://arxiv.org/abs/2501.11319)|[![Star](https://img.shields.io/github/stars/bytedance/StyleSSP.svg?style=social&label=Star)](https://github.com/bytedance/StyleSSP)|CVPR 2025|
|[SigStyle: Signature Style Transfer via Personalized Text-to-Image Models](https://arxiv.org/abs/2502.13997)|[![Star](https://img.shields.io/github/stars/wangyePHD/SigStyle.svg?style=social&label=Star)](https://github.com/wangyePHD/SigStyle)|AAAI 2025|
|[Attention Distillation: A Unified Approach to Visual Characteristics Transfer](https://arxiv.org/abs/2502.20235)|[![Star](https://img.shields.io/github/stars/xugao97/AttentionDistillation.svg?style=social&label=Star)](https://github.com/xugao97/AttentionDistillation)|CVPR 2025|
|[SEMANTIX: AN ENERGY-GUIDED SAMPLER FOR SEMANTIC STYLE TRANSFER](https://arxiv.org/abs/2503.22344)|-|ICLR 2025|
|[Training Free Stylized Abstraction](https://arxiv.org/abs/2505.22663)|[![Star](https://img.shields.io/github/stars/Kartik-3004/TF-SA.svg?style=social&label=Star)](https://github.com/Kartik-3004/TF-SA)|May, 2025|
|[TeleStyle V2: Beyond Content-Preserving Style Transfer with Self-Distillation and Distribution-Matching-Distillation](https://arxiv.org/abs/2606.20709)|[![Star](https://img.shields.io/github/stars/Tele-AI/TeleStyleV2.svg?style=social&label=Star)](https://github.com/Tele-AI/TeleStyleV2)|Jun., 2026|
|[Diffusion in Style](https://openaccess.thecvf.com/content/ICCV2023/papers/Everaert_Diffusion_in_Style_ICCV_2023_paper.pdf)|-|ICCV 2023|
|[Diffusion-Enhanced PatchMatch: A Framework for Arbitrary Style Transfer with Diffusion Models](https://openaccess.thecvf.com/content/CVPR2023W/GCV/papers/Hamazaspyan_Diffusion-Enhanced_PatchMatch_A_Framework_for_Arbitrary_Style_Transfer_With_Diffusion_CVPRW_2023_paper.pdf)|-|CVPR 2023 WorkShop|
|[FreSCo: Joint Frequency-Aware and Spatial Control for Image Zero-Shot Style Transfer](https://dl.acm.org/doi/pdf/10.1145/3805622.3810798)|-|ICMR 2026|

## LoRA-Based Methods
| Title | Github | Pub. & Date |
| :--- | :---: | :---: |
|[ZipLoRA: Any Subject in Any Style by Effectively Merging LoRAs](https://arxiv.org/abs/2311.13600)|-|Nov., 2023|
|[Implicit Style-Content Separation using B-LoRA](https://arxiv.org/abs/2403.14572)|[![Star](https://img.shields.io/github/stars/yardenfren1996/B-LoRA.svg?style=social&label=Star)](https://github.com/yardenfren1996/B-LoRA)|ECCV 2024|
|[B4M: Breaking Low-Rank Adapter for Making Content-Style Customization](https://arxiv.org/abs/2403.19456)|[![Star](https://img.shields.io/github/stars/ICTMCG/Break-for-make.svg?style=social&label=Star)](https://github.com/ICTMCG/Break-for-make)|ACM ToG 2025|
|[Customizing Text-to-Image Models with a Single Image Pair](https://arxiv.org/abs/2405.01536)|[![Star](https://img.shields.io/github/stars/PairCustomization/PairCustomization.svg?style=social&label=Star)](https://github.com/PairCustomization/PairCustomization)|SIGGRAPH Asia 2024|
|[UnZipLoRA: Separating Content and Style from a Single Image](https://arxiv.org/abs/2412.04465)|-|Dec., 2024|
|[K-LoRA: Unlocking Training-Free Fusion of Any Subject and Style LoRAs](https://arxiv.org/abs/2502.18461)|[![Star](https://img.shields.io/github/stars/HVision-NKU/K-LoRA.svg?style=social&label=Star)](https://github.com/HVision-NKU/K-LoRA)|Feb., 2025|
|[ConsisLoRA: Enhancing Content and Style Consistency for LoRA-based Style Transfer](https://arxiv.org/abs/2503.10614?)|[![Star](https://img.shields.io/github/stars/000linlin/ConsisLoRA.svg?style=social&label=Star)](https://github.com/000linlin/ConsisLoRA)|Mar., 2025|
|[Only-Style: Stylistic Consistency in Image Generation without Content Leakage](https://arxiv.org/abs/2506.09916)|[![Star](https://img.shields.io/github/stars/TilemahosAravanis/Only-Style.svg?style=social&label=Star)](https://github.com/TilemahosAravanis/Only-Style)|Jun., 2025|
|[QR-LoRA: Efficient and Disentangled Fine-tuning via QR Decomposition for Customized Generation](https://arxiv.org/abs/2507.04599)|[![Star](https://img.shields.io/github/stars/luna-ai-lab/QR-LoRA.svg?style=social&label=Star)](https://github.com/luna-ai-lab/QR-LoRA)|ICCV 2025|
|[Subject or Style: Adaptive and Training-Free Mixture of LoRAs](https://arxiv.org/abs/2508.02165)|-|Aug., 2025|
|[CRAFT-LoRA: Content-Style Personalization via Rank-Constrained Adaptation and Training-Free Fusion](https://arxiv.org/abs/2602.18936)|-|Feb., 2026|
|[Compressing Image Style Training into a Single Model Forward](https://arxiv.org/pdf/2606.13809)|-|Jun., 2026|

# 📍 Video Synthesis
| Title | Github | Pub. & Date |
| :--- | :---: | :---: |
|[Style-A-Video: Agile Diffusion for Arbitrary Text-based Video Style Transfer](https://arxiv.org/abs/2305.05464)|-|IEEE Signal Processing Letters|
|[StyleCrafter: Enhancing Stylized Text-to-Video Generation with Style Adapter](https://arxiv.org/abs/2312.00330)|[![Star](https://img.shields.io/github/stars/GongyeLiu/StyleCrafter.svg?style=social&label=Star)](https://github.com/GongyeLiu/StyleCrafter)|SIGGRAPH Asia 2024 (Journal Track)|
|[StyleMaster: Stylize Your Video with Artistic Generation and Translation](https://arxiv.org/abs/2412.07744)|[![Star](https://img.shields.io/github/stars/KwaiVGI/StyleMaster.svg?style=social&label=Star)](https://github.com/KwaiVGI/StyleMaster)|CVPR 2025|
|[Rerender A Video: Zero-Shot Text-Guided Video-to-Video Translation](https://arxiv.org/abs/2306.07954)|[![Star](https://img.shields.io/github/stars/williamyang1991/Rerender_A_Video.svg?style=social&label=Star)](https://github.com/williamyang1991/Rerender_A_Video)|SIGGRAPH Asia 2023|
|[Pix2Video: Video Editing using Image Diffusion](https://arxiv.org/abs/2303.12688)|[![Star](https://img.shields.io/github/stars/duyguceylan/pix2video.svg?style=social&label=Star)](https://github.com/duyguceylan/pix2video)|ICCV 2023|
|[FateZero: Fusing Attentions for Zero-shot Text-based Video Editing](https://arxiv.org/abs/2303.09535)|[![Star](https://img.shields.io/github/stars/ChenyangQiQi/FateZero.svg?style=social&label=Star)](https://github.com/ChenyangQiQi/FateZero)|ICCV 2023|
|[Tune-A-Video: One-Shot Tuning of Image Diffusion Models for Text-to-Video Generation](https://arxiv.org/abs/2212.11565)|[![Star](https://img.shields.io/github/stars/showlab/Tune-A-Video.svg?style=social&label=Star)](https://github.com/showlab/Tune-A-Video)|ICCV 2023|
|[Video-P2P: Video Editing with Cross-attention Control](https://arxiv.org/abs/2303.04761)|[![Star](https://img.shields.io/github/stars/JIA-Lab-research/Video-P2P.svg?style=social&label=Star)](https://github.com/JIA-Lab-research/Video-P2P)|CVPR 2024|
|[TokenFlow: Consistent Diffusion Features for Consistent Video Editing](https://arxiv.org/abs/2307.10373)|[![Star](https://img.shields.io/github/stars/omerbt/TokenFlow.svg?style=social&label=Star)](https://github.com/omerbt/TokenFlow)|ICLR 2024|
|[Ground-A-Video: Zero-shot Grounded Video Editing using Text-to-image Diffusion Models](https://arxiv.org/abs/2310.01107)|[![Star](https://img.shields.io/github/stars/Ground-A-Video/Ground-A-Video.svg?style=social&label=Star)](https://github.com/Ground-A-Video/Ground-A-Video)|ICLR 2024|
|[FLATTEN: optical FLow-guided ATTENtion for consistent text-to-video editing](https://arxiv.org/abs/2310.05922)|[![Star](https://img.shields.io/github/stars/yrcong/flatten.svg?style=social&label=Star)](https://github.com/yrcong/flatten)|ICLR 2024|
|[FastBlend: a Powerful Model-Free Toolkit Making Video Stylization Easier](https://arxiv.org/abs/2311.09265)|[![Star](https://img.shields.io/github/stars/Artiprocher/sd-webui-fastblend.svg?style=social&label=Star)](https://github.com/Artiprocher/sd-webui-fastblend)|Nov., 2023|
|[Highly Detailed and Temporal Consistent Video Stylization via Synchronized Multi-Frame Diffusion](https://arxiv.org/abs/2311.14343)|-|CGF 2025|
|[RAVE: Randomized Noise Shuffling for Fast and Consistent Video Editing with Diffusion Models](https://arxiv.org/abs/2312.04524)|[![Star](https://img.shields.io/github/stars/RehgLab/RAVE.svg?style=social&label=Star)](https://github.com/RehgLab/RAVE)|CVPR 2024|
|[VidToMe: Video Token Merging for Zero-Shot Video Editing](https://arxiv.org/abs/2312.10656)|[![Star](https://img.shields.io/github/stars/lixirui142/VidToMe.svg?style=social&label=Star)](https://github.com/lixirui142/VidToMe)|CVPR 2024|
|[Diffutoon: High-Resolution Editable Toon Shading via Diffusion Models](https://arxiv.org/abs/2401.16224)|[![Star](https://img.shields.io/github/stars/modelscope/DiffSynth-Studio.svg?style=social&label=Star)](https://github.com/modelscope/DiffSynth-Studio)|IJCAI 2024|
|[Customize-A-Video: One-Shot Motion Customization of Text-to-Video Diffusion Models](https://arxiv.org/abs/2402.14780)|-|ECCV 2024|
|[FRESCO: Spatial-Temporal Correspondence for Zero-Shot Video Translation](https://arxiv.org/abs/2403.12962)|[![Star](https://img.shields.io/github/stars/williamyang1991/FRESCO.svg?style=social&label=Star)](https://github.com/williamyang1991/FRESCO)|CVPR 2024|
|[AnyV2V: A Tuning-Free Framework For Any Video-to-Video Editing Tasks](https://arxiv.org/abs/2403.14468)|[![Star](https://img.shields.io/github/stars/TIGER-AI-Lab/AnyV2V.svg?style=social&label=Star)](https://github.com/TIGER-AI-Lab/AnyV2V)|TMLR 2024|
|[Looking Backward: Streaming Video-to-Video Translation with Feature Banks](https://arxiv.org/abs/2405.15757)|[![Star](https://img.shields.io/github/stars/Jeff-LiangF/streamv2v.svg?style=social&label=Star)](https://github.com/Jeff-LiangF/streamv2v)|May, 2024|
|[Live2Diff: Live Stream Translation via Uni-directional Attention in Video Diffusion Models](https://arxiv.org/abs/2407.08701)|[![Star](https://img.shields.io/github/stars/open-mmlab/Live2Diff.svg?style=social&label=Star)](https://github.com/open-mmlab/Live2Diff)|Jul., 2024|
|[UniVST: A Unified Framework for Training-free Localized Video Style Transfer](https://arxiv.org/abs/2410.20084)|[![Star](https://img.shields.io/github/stars/QuanjianSong/UniVST.svg?style=social&label=Star)](https://github.com/QuanjianSong/UniVST)|TPAMI 2025|
|[AniDoc: Animation Creation Made Easier](https://arxiv.org/abs/2412.14173)|[![Star](https://img.shields.io/github/stars/yihao-meng/AniDoc.svg?style=social&label=Star)](https://github.com/yihao-meng/AniDoc)|Dec., 2024|
|[SOYO: A Tuning-Free Approach for Video Style Morphing via Style-Adaptive Interpolation in Diffusion Models](https://arxiv.org/abs/2503.06998)|-|Mar., 2025|
|[Inversion-Free Video Style Transfer with Trajectory Reset Attention Control and Content-Style Bridging](https://arxiv.org/abs/2503.07363)|-|Mar., 2025|
|[V-Stylist: Video Stylization via Collaboration and Reflection of MLLM Agents](https://arxiv.org/abs/2503.12077)|-|CVPR 2025|
|[FreeViS: Training-free Video Stylization with Inconsistent References](https://arxiv.org/abs/2510.01686)|-|ICLR 2026|
|[PickStyle: Video-to-Video Style Transfer with Context-Style Adapters](https://arxiv.org/abs/2510.07546)|[![Star](https://img.shields.io/github/stars/PickfordAI/pickstyle.svg?style=social&label=Star)](https://github.com/PickfordAI/pickstyle)|ECCV 2026 WorkShop|
|[Zero-Shot Video Translation and Editing with Frame Spatial-Temporal Correspondence](https://arxiv.org/abs/2512.03905)|[![Star](https://img.shields.io/github/stars/Sunnycookies/FRESCO-v2.svg?style=social&label=Star)](https://github.com/Sunnycookies/FRESCO-v2)|Dec., 2025|
|[DreamStyle: A Unified Framework for Video Stylization](https://arxiv.org/abs/2601.02785)|[![Star](https://img.shields.io/github/stars/LemonSky1995/DreamStyle.svg?style=social&label=Star)](https://github.com/LemonSky1995/DreamStyle)|Jan., 2026|
|[OmniTransfer: All-in-one Framework for Spatio-temporal Video Transfer](https://arxiv.org/abs/2601.14250)|[![Star](https://img.shields.io/github/stars/PangzeCheung/OmniTransfer.svg?style=social&label=Star)](https://github.com/PangzeCheung/OmniTransfer)|Jan., 2026|
|[TeleStyle: Content-Preserving Style Transfer in Images and Videos](https://arxiv.org/pdf/2601.20175)|[![Star](https://img.shields.io/github/stars/Tele-AI/TeleStyle.svg?style=social&label=Star)](https://github.com/Tele-AI/TeleStyle)|Jan., 2026|
|[RFDM: Residual Flow Diffusion Model for Efficient Causal Video Editing](https://arxiv.org/abs/2602.06871)|-|CVPR 2026|
|[DiT as Real-Time Rerenderer: Streaming Video Stylization with Autoregressive Diffusion Transformer](https://arxiv.org/abs/2604.13509)|-|Apr., 2026|
|[VISTA: Triplet-Supervised Video Style Transfer with Diffusion Transformers](https://arxiv.org/abs/2605.17312)|-|May, 2026|
|[SANA-Streaming: Real-time Streaming Video Editing with Hybrid Diffusion Transformer](https://arxiv.org/abs/2605.30409)|[![Star](https://img.shields.io/github/stars/NVlabs/Sana.svg?style=social&label=Star)](https://github.com/NVlabs/Sana)|May, 2026|
|[EchoStyle: Unlocking High-Fidelity Video Stylization with Reverse Data Synthesis](https://arxiv.org/abs/2606.25465)|[![Star](https://img.shields.io/github/stars/HKUST-C4G/EchoStyle.svg?style=social&label=Star)](https://github.com/HKUST-C4G/EchoStyle)|ECCV 2026|
|[Stylized Video Generation via Decoupled Data Synthesis and Gated Style Token Injection](https://link.springer.com/chapter/10.1007/978-3-032-37235-2_2)|-|ECCV 2026|

# 📍 3D Generation
| Title | Github | Pub. & Date |
| :--- | :---: | :---: |
|[TEXTure: Text-Guided Texturing of 3D Shapes](https://arxiv.org/abs/2302.01721)|[![Star](https://img.shields.io/github/stars/TEXTurePaper/TEXTurePaper.svg?style=social&label=Star)](https://github.com/TEXTurePaper/TEXTurePaper)|SIGGRAPH 2023|
|[Paint-it: Text-to-Texture Synthesis via Deep Convolutional Texture Map Optimization and Physically-Based Rendering](https://arxiv.org/abs/2312.11360)|[![Star](https://img.shields.io/github/stars/postech-ami/paint-it.svg?style=social&label=Star)](https://github.com/postech-ami/paint-it)|CVPR 2024|
|[TextureDreamer: Image-guided Texture Synthesis through Geometry-aware Diffusion](https://arxiv.org/abs/2401.09416)|-|CVPR 2024|
|[StyleTex: Style Image-Guided Texture Generation for 3D Models](https://arxiv.org/abs/2411.00399)|-|SIGGRAPH Asia 2024|
|[Style3D: Attention-guided Multi-view Style Transfer for 3D Object Generation](https://arxiv.org/abs/2412.03571)|-|Dec., 2024|
|[StyleMe3D: Stylization with Disentangled Priors by Multiple Encoders on 3D Gaussians](https://arxiv.org/abs/2504.15281?)|[![Star](https://img.shields.io/github/stars/AIGCResearch/styleme3d.svg?style=social&label=Star)](https://github.com/AIGCResearch/styleme3d)|Apr., 2024|

# 📍 Style Dataset
| Title | Dataset | Github | Pub. & Date |
| :--- | :---: | :---: | :---: |
|[UnlearnCanvas: A Stylized Image Dataset to Benchmark Machine Unlearning for Diffusion Models](https://arxiv.org/abs/2402.11846)|UnlearnCanvas ✅|[![Star](https://img.shields.io/github/stars/OPTML-Group/UnlearnCanvas.svg?style=social&label=Star)](https://github.com/OPTML-Group/UnlearnCanvas)|NeurIPS 2024 D&B Track|
|[StyleBooth: Image Style Editing with Multimodal Instruction](https://arxiv.org/abs/2404.12154)|StyleBooth dataset ✅|[![Star](https://img.shields.io/github/stars/modelscope/scepter.svg?style=social&label=Star)](https://github.com/modelscope/scepter)|Apr., 2024|
|[StyleShot: A Snapshot on Any Style](https://arxiv.org/abs/2407.01414)|StyleGallery ✅ / StyleBench ✅|[![Star](https://img.shields.io/github/stars/open-mmlab/StyleShot.svg?style=social&label=Star)](https://github.com/open-mmlab/StyleShot)|Jul., 2024|
|[CSGO: Content-Style Composition in Text-to-Image Generation](https://arxiv.org/abs/2408.16766)|IMAGStyle ❌|[![Star](https://img.shields.io/github/stars/instantX-research/CSGO.svg?style=social&label=Star)](https://github.com/instantX-research/CSGO)|Aug., 2024|
|[StyleTokenizer: Defining Image Style by a Single Instance for Controlling Diffusion Models](https://arxiv.org/abs/2409.02543)|Style30K ✅|[![Star](https://img.shields.io/github/stars/alipay/style-tokenizer.svg?style=social&label=Star)](https://github.com/alipay/style-tokenizer)|ECCV 2024|
|[V-Stylist: Video Stylization via Collaboration and Reflection of MLLM Agents](https://arxiv.org/abs/2503.12077)|TVSBench ❌|-|CVPR 2025|
|[OmniStyle: Filtering High Quality Style Transfer Data at Scale](https://arxiv.org/abs/2505.14028)|OmniStyle-1M ❌ / OmniStyle-150K ✅|-|CVPR 2025|
|[OmniStyle2: Learning to Stylize by Learning to Destylize](https://arxiv.org/abs/2509.05970)|DeStyle-350K ✅ / BCS-Bench ❌|-|Sep., 2025|
|[PickStyle: Video-to-Video Style Transfer with Context-Style Adapters](https://arxiv.org/abs/2510.07546)|PickStyle-Dataset ✅|[![Star](https://img.shields.io/github/stars/PickfordAI/pickstyle.svg?style=social&label=Star)](https://github.com/PickfordAI/pickstyle)|ECCV 2026 WorkShop|
|[Mixture of Style Experts for Diverse Image Stylization](https://openaccess.thecvf.com/content/CVPR2026/papers/Zhu_Mixture_of_Style_Experts_for_Diverse_Image_Stylization_CVPR_2026_paper.pdf)|StyleExpert-500K ❌ / StyleExpert-40K ✅|[![Star](https://img.shields.io/github/stars/HVision-NKU/StyleExpert.svg?style=social&label=Star)](https://github.com/HVision-NKU/StyleExpert)|CVPR 2026|
|[MegaStyle: Constructing Diverse and Scalable Style Dataset via Consistent Text-to-Image Style Mapping](https://arxiv.org/abs/2604.08364)|MegaStyle-1.4M ✅|[![Star](https://img.shields.io/github/stars/Tencent/MegaStyle.svg?style=social&label=Star)](https://github.com/Tencent/MegaStyle)|CVPR 2026|
|[VISTA: Triplet-Supervised Video Style Transfer with Diffusion Transformers](https://arxiv.org/abs/2605.17312)|VISTA-1000 ✅|-|May, 2026|
|[EchoStyle: Unlocking High-Fidelity Video Stylization with Reverse Data Synthesis](https://arxiv.org/abs/2606.25465)|V-Style20k ❌|[![Star](https://img.shields.io/github/stars/HKUST-C4G/EchoStyle.svg?style=social&label=Star)](https://github.com/HKUST-C4G/EchoStyle)|ECCV 2026|
|[Stylized Video Generation via Decoupled Data Synthesis and Gated Style Token Injection](https://link.springer.com/chapter/10.1007/978-3-032-37235-2_2)|MoStyle-5K ❌|-|ECCV 2026|
|[MegaStyle++: Scaling Image Style Space through Hierarchical Style Definition](https://arxiv.org/abs/2609.01423)|MegaStyle++-8M ✅|[![Star](https://img.shields.io/github/stars/Tencent/MegaStyle.svg?style=social&label=Star)](https://github.com/Tencent/MegaStyle)|Sep., 2026|

# 📍 Related Research and Surveys
| Title | Github | Pub. & Date |
| :--- | :---: | :---: |
|[Image Style Transfer Using Convolutional Neural Networks](https://www.cv-foundation.org/openaccess/content_cvpr_2016/papers/Gatys_Image_Style_Transfer_CVPR_2016_paper.pdf)|[![Star](https://img.shields.io/github/stars/superb20/Image-Style-Transfer-Using-Convolutional-Neural-Networks.svg?style=social&label=Star)](https://github.com/superb20/Image-Style-Transfer-Using-Convolutional-Neural-Networks)|CVPR 2016|
|[StyleBank: An Explicit Representation for Neural Image Style Transfer](https://arxiv.org/abs/1703.09210)|-|CVPR 2017|
|[StyleCLIPDraw: Coupling Content and Style in Text-to-Drawing Translation](https://arxiv.org/abs/2202.12362)|-|IJCAI 2022|
|[Simple Disentanglement of Style and Content in Visual Representations](https://arxiv.org/abs/2302.09795)|[![Star](https://img.shields.io/github/stars/lilianngweta/PISCO.svg?style=social&label=Star)](https://github.com/lilianngweta/PISCO)|ICML 2023|
|[Text2Video-Zero: Text-to-Image Diffusion Models are Zero-Shot Video Generators](https://arxiv.org/abs/2303.13439)|[![Star](https://img.shields.io/github/stars/Picsart-AI-Research/Text2Video-Zero.svg?style=social&label=Star)](https://github.com/Picsart-AI-Research/Text2Video-Zero)|ICCV 2023|
|[VideoComposer: Compositional Video Synthesis with Motion Controllability](https://arxiv.org/abs/2306.02018)|[![Star](https://img.shields.io/github/stars/ali-vilab/videocomposer.svg?style=social&label=Star)](https://github.com/ali-vilab/videocomposer)|ICCV 2023|
|[UnlearnCanvas: A Stylized Image Dataset to Benchmark Machine Unlearning for Diffusion Models](https://arxiv.org/abs/2402.11846)|[![Star](https://img.shields.io/github/stars/OPTML-Group/UnlearnCanvas.svg?style=social&label=Star)](https://github.com/OPTML-Group/UnlearnCanvas)|NeurIPS 2024 D&B Track|
|[Diffusion Model-Based Image Editing: A Survey](https://arxiv.org/abs/2402.17525)|-|Feb., 2024|
|[Diffusion-Based Visual Art Creation: A Survey and New Perspectives](https://arxiv.org/abs/2408.12128)|-|Sep., 2024|
|[Conditional Image Synthesis with Diffusion Models: A Survey](https://arxiv.org/abs/2409.19365)|[![Star](https://img.shields.io/github/stars/zju-pi/Awesome-Conditional-Diffusion-Models.svg?style=social&label=Star)](https://github.com/zju-pi/Awesome-Conditional-Diffusion-Models)|Sep., 2024|
|[Advances in 3D Neural Stylization: A Survey](https://arxiv.org/abs/2311.18328)|[![Star](https://img.shields.io/github/stars/chenyingshu/advances_3d_neural_stylization.svg?style=social&label=Star)](https://github.com/chenyingshu/advances_3d_neural_stylization)|IJCV 2025|
