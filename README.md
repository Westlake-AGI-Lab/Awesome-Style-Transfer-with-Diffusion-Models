<!-- <div align="center">
<h2> Awesome Style Transfer with Diffusion Models </h2> 
</div> -->
# 🥳Awesome Style Transfer with Diffusion Models [![Awesome](https://awesome.re/badge.svg)](https://awesome.re) 

# 🤗 Introduction
- This repository contains a curated list of **Style Transfer with Diffusion Models**. The resources are organized into two main categories: Image Synthesis and Video Synthesis. 
In the context of Image Style Transfer, the techniques can be categorized into two primary types: text-driven style transfer and image-driven style transfer.

<p align="center">
  <img src="assets/teaser1.jpg" width="80%">
</p>

- We welcome any contributions and suggestions to our repository or the addition of your own work. Feel free to make a pull request or leave your comments!!

# 📋 Contents
- [🤗 Introduction](#-introduction)
- [📋 Contents](#-contents)
- [💘 Tips](#-tips)
- [📍 Image Synthesis](#-image-synthesis)
  - [Text-Driven Style Transfer](#text-driven-style-transfer)
    - [Image-Encoder Based](#image-encoder-based)
    - [Textual-Inversion Based](#textual-inversion-based)
    - [Swap Features In Attention Layer](#swap-features-in-attention-layer)
    - [Fine-tune Methods](#fine-tune-methods)
    - [Training-free Methods](#training-free-methods)
  - [Image-Driven Style Transfer](#image-driven-style-transfer)
    - [Text-Guided Style Transfer](#text-guided-style-transfer)
    - [None Diffusion Models](#none-diffusion-models)
- [📍 Video Synthesis](#-video-synthesis)
  - [Text-to-Video Generation](#text-to-video-generation)
  - [Video-to-Video Translation](#video-to-video-translation)
- [📍 3D Generation](#-3d-generation)
- [📍 Related Research and Surveys](#-related-research-and-surveys)


# 💘 Tips
- **✅ Paper searching via catatogue**: directly clicking the content of the catatogue to select the area of your research and browse related papers.
- **✅ Paper searching via author name**: Free feel to search papers of a specific author via `ctrl/cmd + F` and then type the author name. The dropdown list of authors will automatically expand when searching.

# 📍 Image Synthesis
## Text-Driven Style Transfer
### Image-Encoder Based

+ **IP-Adapter: Text Compatible Image Prompt Adapter for Text-to-Image Diffusion Models** (13 Aug 2023) <details><summary>Hu Ye, Jun Zhang et al.</summary>Hu Ye, Jun Zhang, Sibo Liu, Xiao Han, Wei Yang</details>
[![Paper](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2308.06721)
[![Code](https://img.shields.io/github/stars/tencent-ailab/IP-Adapter.svg?style=social&label=Star)](https://github.com/tencent-ailab/IP-Adapter)
[![Page](https://img.shields.io/badge/Page-green)](https://ip-adapter.github.io/)

+ **StyleAdapter: A Unified Stylized Image Generation Model** (4 Sep 2023) <details><summary>Zhouxia Wang, Xintao Wang et al.</summary>Zhouxia Wang, Xintao Wang, Liangbin Xie, Zhongang Qi, Ying Shan, Wenping Wang, Ping Luo</details>
[![Paper](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2309.01770)
[![Page](https://img.shields.io/badge/Page-green)]()

+ **ArtAdapter: Text-to-Image Style Transfer using Multi-Level Style Encoder and Explicit Adaptation** (4 Dec 2023) <details><summary>[CVPR 2024] Dar-Yen Chen, Hamish Tennent et al.</summary>Dar-Yen Chen, Hamish Tennent, Ching-Wen Hsu</details>
[![Paper](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2312.02109)
[![Code](https://img.shields.io/github/stars/cardinalblue/ArtAdapter.svg?style=social&label=Star)](https://github.com/cardinalblue/ArtAdapter)
[![Page](https://img.shields.io/badge/Page-green)](https://cardinalblue.github.io/artadapter.github.io/)

+ **InstantStyle: Free Lunch towards Style-Preserving in Text-to-Image Generation** (3 Apr 2024) <details><summary>Haofan Wang, Matteo Spinelli et al.</summary>Haofan Wang, Matteo Spinelli, Qixun Wang, Xu Bai, Zekui Qin, Anthony Chen</details>
[![Paper](https://img.shields.io/badge/arXiv-b31b1b.svg)]()
[![Code](https://img.shields.io/github/stars/instantX-research/InstantStyle.svg?style=social&label=Star)](https://github.com/instantX-research/InstantStyle)
[![Page](https://img.shields.io/badge/Page-green)](https://instantstyle.github.io/)

+ **DEADiff: An Efficient Stylization Diffusion Model with Disentangled Representations** (11 Mar 2024) <details><summary>[CVPR 2024] Tianhao Qi, Shancheng Fang et al.</summary>Tianhao Qi, Shancheng Fang, Yanze Wu, Hongtao Xie, Jiawei Liu, Lang Chen, Qian He, Yongdong Zhang</details>
[![Paper](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2403.06951)
[![Code](https://img.shields.io/github/stars/bytedance/DEADiff.svg?style=social&label=Star)](https://github.com/bytedance/DEADiff)
[![Page](https://img.shields.io/badge/Page-green)](https://tianhao-qi.github.io/DEADiff/)

+ **StyleMaster: Towards Flexible Stylized Image Generation with Diffusion Models** (24 May 2024) <details><summary>Chengming Xu, Kai Hu et al.</summary>Chengming Xu, Kai Hu, Donghao Luo, Jiangning Zhang, Wei Li, Yanhao Ge, Chengjie Wang</details>
[![Paper](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2405.15287v1)

+ **StyleShot: A Snapshot on Any Style** (1 Jul 2024) <details><summary>Junyao Gao, Yanchen Liu et al.</summary>Junyao Gao, Yanchen Liu, Yanan Sun, Yinhao Tang, Yanhong Zeng, Kai Chen, Cairong Zhao</details>
[![Paper](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2407.01414)
[![Code](https://img.shields.io/github/stars/open-mmlab/StyleShot.svg?style=social&label=Star)](https://github.com/open-mmlab/StyleShot)
[![Page](https://img.shields.io/badge/Page-green)](https://styleshot.github.io/)

+ **CSGO: Content-Style Composition in Text-to-Image Generation** (29 Aug 2024) <details><summary>Peng Xing, Haofan Wang et al.</summary>Peng Xing, Haofan Wang, Yanpeng Sun, Qixun Wang, Xu Bai, Hao Ai, Renyuan Huang, Zechao Li</details>
[![Paper](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2408.16766)
[![Code](https://img.shields.io/github/stars/instantX-research/CSGO.svg?style=social&label=Star)](https://github.com/instantX-research/CSGO)
[![Page](https://img.shields.io/badge/Page-green)](https://csgo-gen.github.io/)

+ **StyleTokenizer: Defining Image Style by a Single Instance for Controlling Diffusion Models** (4 Sep 2024) <details><summary>[ECCV 2024] Wen Li, Muyuan Fang et al.</summary>Wen Li, Muyuan Fang, Cheng Zou, Biao Gong, Ruobing Zheng, Meng Wang, Jingdong Chen, Ming Yang</details>
[![Paper](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2409.02543)
[![Code](https://img.shields.io/github/stars/alipay/style-tokenizer.svg?style=social&label=Star)](https://github.com/alipay/style-tokenizer) 

+ **StyleStudio: Text-Driven Style Transfer with Selective Control of Style Elements** (11 Dec 2024) <details><summary>[CVPR 2025] Mingkun Lei, Xue Song et al.</summary>Mingkun Lei, Xue Song, Beier Zhu, Hao Wang, Chi Zhang</details>
[![Paper](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2412.08503)
[![Code](https://img.shields.io/github/stars/Westlake-AGI-Lab/StyleStudio.svg?style=social&label=Star)](https://github.com/Westlake-AGI-Lab/StyleStudio) 
[![Page](https://img.shields.io/badge/Page-green)](https://stylestudio-official.github.io/)

+ **EasyRef: Omni-Generalized Group Image Reference for Diffusion Models via Multimodal LLM** (12 Dec 2024) <details><summary> Zhuofan Zong, Dongzhi Jiang et al.</summary>Zhuofan Zong, Dongzhi Jiang, Bingqi Ma, Guanglu Song, Hao Shao, Dazhong Shen, Yu Liu, Hongsheng Li</details>
[![Paper](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2412.09618v1)


+ **ArtCrafter: Text-Image Aligning Style Transfer via Embedding Reframing** (3 Jan 2025) <details><summary> Nisha Huang, Kaer Huang et al.</summary>Nisha Huang, Kaer Huang, Yifan Pu, Jiangshan Wang, Jie Guo, Yiqiang Yan, Xiu Li</details>
[![Paper](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2501.02064)

+ **Less is More: Masking Elements in Image Condition Features Avoids Content Leakages in Style Transfer Diffusion Models** (11 Feb 2025) <details><summary>[ICLR 2025] Lin Zhu, Xinbing Wang et al.</summary>Lin Zhu, Xinbing Wang, Chenghu Zhou, Qinying Gu, Nanyang Ye</details>
[![Paper](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2502.07466)
[![Code](https://img.shields.io/github/stars/LinLLLL/MaskST.svg?style=social&label=Star)](https://github.com/LinLLLL/MaskST)

### Textual-Inversion Based

+ **An Image is Worth One Word: Personalizing Text-to-Image Generation using Textual Inversion** (2 Aug 2022) <details><summary>[ICLR 2023] Rinon Gal, Yuval Alaluf et al.</summary>Rinon Gal, Yuval Alaluf, Yuval Atzmon, Or Patashnik, Amit H. Bermano, Gal Chechik, Daniel Cohen-Or</details>
[![Paper](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2208.01618)
[![Code](https://img.shields.io/github/stars/rinongal/textual_inversion.svg?style=social&label=Star)](https://github.com/rinongal/textual_inversion)
[![Page](https://img.shields.io/badge/Page-green)](https://textual-inversion.github.io/)

+ **Inversion-Based Style Transfer with Diffusion Models** (23 Nov 2022) <details><summary>[CVPR 2023] Yuxin Zhang, Nisha Huang et al.</summary>Yuxin Zhang, Nisha Huang, Fan Tang, Haibin Huang, Chongyang Ma, Weiming Dong, Changsheng Xu</details>
[![Paper](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2211.13203)
[![Code](https://img.shields.io/github/stars/zyxElsa/InST.svg?style=social&label=Star)](https://github.com/zyxElsa/InST)

+ **An Image is Worth Multiple Words: Multi-attribute Inversion for Constrained Text-to-Image Synthesis** (20 Nov 2023) <details><summary>Aishwarya Agarwal et al.</summary>Aishwarya Agarwal, Srikrishna Karanam, Tripti Shukla, Balaji Vasan Srinivasan</details>
[![Paper](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2311.11919)

### Swap Features In Attention Layer

+ **Cross-Image Attention for Zero-Shot Appearance Transfer** (6 Nov 2023) <details><summary>[SIGGRAPH 2024] Yuval Alaluf, Daniel Garibi et al.</summary>Yuval Alaluf, Daniel Garibi, Or Patashnik, Hadar Averbuch-Elor, Daniel Cohen-Or</details>
[![Paper](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2311.03335)
[![Code](https://img.shields.io/github/stars/garibida/cross-image-attention.svg?style=social&label=Star)](https://github.com/garibida/cross-image-attention)
[![Page](https://img.shields.io/badge/Page-green)](https://garibida.github.io/cross-image-attention/)

+ **Style Aligned Image Generation via Shared Attention** (4 Dec 2023) <details><summary>[CVPR 2024] Amir Hertz, Andrey Voynov et al.</summary>Amir Hertz, Andrey Voynov, Shlomi Fruchter, Daniel Cohen-Or</details>
[![Paper](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2312.02133)
[![Code](https://img.shields.io/github/stars/google/style-aligned.svg?style=social&label=Star)](https://github.com/google/style-aligned/)
[![Page](https://img.shields.io/badge/Page-green)](https://style-aligned-gen.github.io/)

+ **Visual Style Prompting with Swapping Self-Attention** (20 Feb 2024) <details><summary>Jaeseok Jeong, Junho Kim et al.</summary>Jaeseok Jeong, Junho Kim, Yunjey Choi, Gayoung Lee, Youngjung Uh</details>
[![Paper](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2402.12974)
[![Code](https://img.shields.io/github/stars/naver-ai/Visual-Style-Prompting.svg?style=social&label=Star)](https://github.com/naver-ai/Visual-Style-Prompting)
[![Page](https://img.shields.io/badge/Page-green)](https://curryjung.github.io/VisualStylePrompt/)

+ **StyleGuide: Crafting visual style prompting with negative visual query guidance**  
[![Paper](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://openreview.net/pdf?id=618qfjvSt9)

+ **Training-free Color-Style Disentanglement for Constrained Text-to-Image Synthesis** <details><summary>Yujia Gu, Haofeng Li et al.</summary>Yujia Gu, Haofeng Li, Xinyu Fang, Zihan Peng, Yinan Peng</details> 
[![Paper](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2409.02429)

### Fine-tune Methods & LoRA-Based Methods

+ **Diffusion in Style** <details><summary>[ICCV 2023] Martin Nicolas Everaert, Marco Bocchio et al.</summary>Martin Nicolas Everaert, Marco Bocchio, Sami Arpa, Sabine Süsstrunk, Radhakrishna Achanta</details>
[![Paper](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://openaccess.thecvf.com/content/ICCV2023/papers/Everaert_Diffusion_in_Style_ICCV_2023_paper.pdf)
[![Page](https://img.shields.io/badge/Page-green)](https://ivrl.github.io/diffusion-in-style/)

+ **StyleDrop: Text-to-Image Generation in Any Style** (1 Jun 2023) <details><summary>[NeurIPS 2023] Kihyuk Sohn, Nataniel Ruiz et al.</summary>Kihyuk Sohn, Nataniel Ruiz, Kimin Lee, Daniel Castro Chin, Irina Blok, Huiwen Chang, Jarred Barber, Lu Jiang, Glenn Entis, Yuanzhen Li, Yuan Hao, Irfan Essa, Michael Rubinstein, Dilip Krishnan</details>
[![Paper](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2306.00983)
[![Page](https://img.shields.io/badge/Page-green)](https://styledrop.github.io/)

+ **DreamStyler: Paint by Style Inversion with Text-to-Image Diffusion Models** (13 Sep 2023) <details><summary>[AAAI 2024] Namhyuk Ahn, Junsoo Lee et al.</summary>Namhyuk Ahn, Junsoo Lee, Chunggi Lee, Kunhee Kim, Daesik Kim, Seung-Hun Nam, Kibeom Hong</details>
[![Paper](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2309.06933)
[![Code](https://img.shields.io/github/stars/webtoon/dreamstyler.svg?style=social&label=Star)](https://github.com/webtoon/dreamstyler)
[![Page](https://img.shields.io/badge/Page-green)](https://nmhkahn.github.io/dreamstyler/)

+ **ControlStyle: Text-Driven Stylized Image Generation Using Diffusion Priors** (9 Nov 2023) <details><summary>[MM 2023] Jingwen Chen, Yingwei Pan et al.</summary>Jingwen Chen, Yingwei Pan, Ting Yao, Tao Mei</details>
[![Paper](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2311.05463)

+ **ZipLoRA: Any Subject in Any Style by Effectively Merging LoRAs** (22 Nov 2023) <details><summary>Viraj Shah, Nataniel Ruiz et al.</summary>Viraj Shah, Nataniel Ruiz, Forrester Cole, Erika Lu, Svetlana Lazebnik, Yuanzhen Li, Varun Jampani</details>
[![Paper](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2311.13600)
[![Page](https://img.shields.io/badge/Page-green)](https://ziplora.github.io/)

+ **Implicit Style-Content Separation using B-LoRA** (21 Mar 2024) <details><summary>[ECCV 2024] Yarden Frenkel, Yael Vinker et al.</summary>Yarden Frenkel, Yael Vinker, Ariel Shamir, Daniel Cohen-Or</details>
[![Paper](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2403.14572)
[![Code](https://img.shields.io/github/stars/yardenfren1996/B-LoRA.svg?style=social&label=Star)](https://github.com/yardenfren1996/B-LoRA)
[![Page](https://img.shields.io/badge/Page-green)](https://b-lora.github.io/B-LoRA/)

+ **Frequency-Controlled Diffusion Model for Versatile Text-Guided Image-to-Image Translation** (3 Jul 2024) <details><summary>[AAAI 2024] Xiang Gao, Zhengbo Xu et al.</summary>Xiang Gao, Zhengbo Xu, Junhan Zhao, Jiaying Liu</details>
[![Paper](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2407.03006)

+ **UnZipLoRA: Separating Content and Style from a Single Image** (5 Dec 2024) <details><summary>Chang Liu, Viraj Shah et al.</summary>Chang Liu, Viraj Shah, Aiyu Cui, Svetlana Lazebnik</details>
[![Paper](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2412.04465)
[![Page](https://img.shields.io/badge/Page-green)](https://unziplora.github.io/)

+ **K-LoRA: Unlocking Training-Free Fusion of Any Subject and Style LoRAs** (25 Feb 2025) <details><summary>Ziheng Ouyang et al.</summary>Ziheng Ouyang, Zhen Li, Qibin Hou</details>
[![Paper](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2502.18461)
[![Code](https://img.shields.io/github/stars/HVision-NKU/K-LoRA.svg?style=social&label=Star)](https://github.com/HVision-NKU/K-LoRA)
[![Page](https://img.shields.io/badge/Page-green)](https://k-lora.github.io/K-LoRA.io/)

+ **ConsisLoRA: Enhancing Content and Style Consistency for LoRA-based Style Transfer** (13 Mar 2025) <details><summary>Bolin Chen et al.</summary>Bolin Chen, Baoquan Zhao, Haoran Xie, Yi Cai, Qing Li, Xudong Mao</details>
[![Paper](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2503.10614?)
[![Code](https://img.shields.io/github/stars/000linlin/ConsisLoRA.svg?style=social&label=Star)](https://github.com/000linlin/ConsisLoRA)
[![Page](https://img.shields.io/badge/Page-green)](https://consislora.github.io)

### Training-free Methods
+ **FreeDoM: Training-Free Energy-Guided Conditional Diffusion Model** (17 Mar 2023) <details><summary>[ICCV 2023] Jiwen Yu, Yinhuai Wang et al.</summary>Jiwen Yu, Yinhuai Wang, Chen Zhao, Bernard Ghanem, Jian Zhang</details>
[![Paper](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2303.09833)
[![Code](https://img.shields.io/github/stars/vvictoryuki/FreeDoM.svg?style=social&label=Star)](https://github.com/vvictoryuki/FreeDoM)

+ **VectorPainter: Advanced Stylized Vector Graphics Synthesis Using Stroke-Style Priors** (5 May 2024) <details><summary>[ICME 2025] Juncheng Hu et al.</summary>Juncheng Hu, Ximing Xing, Jing Zhang, Qian Yu</details>
[![Paper](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2405.02962)

+ **Training Free Stylized Abstraction** (28 May 2025) <details><summary>Aimon Rahman et al.</summary>Aimon Rahman, Kartik Narayan, Vishal M. Patel</details>
[![Paper](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2505.22663)
[![Code](https://img.shields.io/github/stars/Kartik-3004/TF-SA.svg?style=social&label=Star)](https://github.com/Kartik-3004/TF-SA)
[![Page](https://img.shields.io/badge/Page-green)](https://kartik-3004.github.io/TF-SA/)

#### Test-time optimization
+ **RB-Modulation: Training-Free Personalization of Diffusion Models using Stochastic Optimal Control** (ICLR 2025) <details><summary>Litu Rout, Yujia Chen et al.</summary>Litu Rout, Yujia Chen, Nataniel Ruiz, Abhishek Kumar, Constantine Caramanis, Sanjay Shakkottai, Wen-Sheng Chu</details>
[![Paper](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2405.17401)
[![Code](https://img.shields.io/github/stars/google/RB-Modulation.svg?style=social&label=Star)](https://github.com/google/RB-Modulation)
[![Page](https://img.shields.io/badge/Page-green)](https://rb-modulation.github.io/)

+ **Attention Distillation: A Unified Approach to Visual Characteristics Transfer** (CVPR 2025) <details><summary>Yang Zhou et al.</summary>Yang Zhou, Xu Gao, Zichong Chen, Hui Huang</details>
[![Paper](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2502.20235)
[![Code](https://img.shields.io/github/stars/xugao97/AttentionDistillation.svg?style=social&label=Star)](https://github.com/xugao97/AttentionDistillation)
[![Page](https://img.shields.io/badge/Page-green)](https://xugao97.github.io/AttentionDistillation/)


## Image-Driven Style Transfer

+ **General Image-to-Image Translation with One-Shot Image Guidance** (20 Jul 2023) <details><summary>Bin Cheng, Zuhao Liu et al.</summary>Bin Cheng, Zuhao Liu, Yunbo Peng, Yue Lin</details>
[![Paper](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2307.14352)
[![Code](https://img.shields.io/github/stars/CrystalNeuro/visual-concept-translator.svg?style=social&label=Star)](https://github.com/CrystalNeuro/visual-concept-translator) 

+ **Null-text Guidance in Diffusion Models is Secretly a Cartoon-style Creator** (11 May 2023) <details><summary>[MM 2023] Bin Cheng, Zuhao Liu et al.</summary>Bin Cheng, Zuhao Liu, Yunbo Peng, Yue Lin</details>
[![Paper](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2305.06710)
[![Code](https://img.shields.io/github/stars/NullTextforCartoon/NullTextforCartoon.svg?style=social&label=Star)](https://github.com/NullTextforCartoon/NullTextforCartoon) 
[![Page](https://img.shields.io/badge/Page-green)](https://nulltextforcartoon.github.io/)

+ **StyleDiffusion: Controllable Disentangled Style Transfer via Diffusion Models** (15 Aug 2023) <details><summary>[ICCV 2023] Zhizhong Wang, Lei Zhao et al.</summary>Zhizhong Wang, Lei Zhao, Wei Xing</details>
[![Paper](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2308.07863)

+ **Diffusion-Enhanced PatchMatch: A Framework for Arbitrary Style Transfer with Diffusion Models** <details><summary>[CVPR 2023] Mark Hamazaspyan, Shant Navasardyan</summary>Mark Hamazaspyan, Shant Navasardyan</details>
[![Paper](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://openaccess.thecvf.com/content/CVPR2023W/GCV/papers/Hamazaspyan_Diffusion-Enhanced_PatchMatch_A_Framework_for_Arbitrary_Style_Transfer_With_Diffusion_CVPRW_2023_paper.pdf)

+ **Z-STAR: Zero-shot Style Transfer via Attention Rearrangement** (25 Nov 2023) <details><summary>[CVPR 2024] Yingying Deng et al.</summary>Yingying Deng, Xiangyu He, Fan Tang, Weiming Dong</details>
[![Paper](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2311.16491)
[![Code](https://img.shields.io/github/stars/HolmesShuan/Zero-shot-Style-Transfer-via-Attention-Rearrangement.svg?style=social&label=Star)](https://github.com/HolmesShuan/Zero-shot-Style-Transfer-via-Attention-Rearrangement)

+ **Style Injection in Diffusion: A Training-free Approach for Adapting Large-scale Diffusion Models for Style Transfer** (11 Dec 2023) <details><summary>[CVPR 2024] Jiwoo Chung, Sangeek Hyun et al.</summary>Jiwoo Chung, Sangeek Hyun, Jae-Pil Heo</details>
[![Paper](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2312.09008)
[![Code](https://img.shields.io/github/stars/jiwoogit/StyleID.svg?style=social&label=Star)](https://github.com/jiwoogit/StyleID)
[![Page](https://img.shields.io/badge/Page-green)](https://jiwoogit.github.io/StyleID_site/)

+ **HiCAST: Highly Customized Arbitrary Style Transfer with Adapter Enhanced Diffusion Models** (11 Jan 2024) <details><summary>Hanzhang Wang, Haoran Wang et al.</summary>Hanzhang Wang, Haoran Wang, Jinze Yang, Zhongrui Yu, Zeke Xie, Lei Tian, Xinyan Xiao, Junjun Jiang, Xianming Liu, Mingming Sun</details>
[![Paper](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2312.09008)
[![Code](https://img.shields.io/github/stars/wd1511/HiCAST.svg?style=social&label=Star)](https://github.com/wd1511/HiCAST)

+ **ParaGuide: Guided Diffusion Paraphrasers for Plug-and-Play Textual Style Transfer** (29 Aug 2023) <details><summary>[AAAI 2024] Zachary Horvitz et al.</summary>Zachary Horvitz, Ajay Patel, Chris Callison-Burch, Zhou Yu, Kathleen McKeown</details>
[![Paper](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2308.15459)
[![Code](https://img.shields.io/github/stars/zacharyhorvitz/ParaGuide.svg?style=social&label=Star)](https://github.com/zacharyhorvitz/ParaGuide)

+ **AesFA: An Aesthetic Feature-Aware Arbitrary Neural Style Transfer** (10 Dec 2023) <details><summary>[AAAI 2024] Joonwoo Kwon, Sooyoung Kim et al.</summary>Joonwoo Kwon, Sooyoung Kim, Yuewei Lin, Shinjae Yoo, Jiook Cha</details>
[![Paper](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2312.05928)
[![Code](https://img.shields.io/github/stars/Sooyyoungg/AesFA.svg?style=social&label=Star)](https://github.com/Sooyyoungg/AesFA)

+ **ArtBank: Artistic Style Transfer with Pre-trained Diffusion Model and Implicit Style Prompt Bank** (11 Dec 2023) <details><summary>[AAAI 2024] Zhanjie Zhang, Quanwei Zhang et al.</summary>Zhanjie Zhang, Quanwei Zhang, Guangyuan Li, Wei Xing, Lei Zhao, Jiakai Sun, Zehua Lan, Junsheng Luan, Yiling Huang, Huaizhong Lin</details>
[![Paper](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2312.09008)
[![Code](https://img.shields.io/github/stars/Jamie-Cheung/ArtBank.svg?style=social&label=Star)](https://github.com/Jamie-Cheung/ArtBank)

+ **Towards Highly Realistic Artistic Style Transfer via Stable Diffusion with Step-aware and Layer-aware Prompt** (17 Apr 2024) <details><summary>[IJCAI 2024] Zhanjie Zhang, Quanwei Zhang et al.</summary>Zhanjie Zhang, Quanwei Zhang, Huaizhong Lin, Wei Xing, Juncheng Mo, Shuaicheng Huang, Jinheng Xie, Guangyuan Li, Junsheng Luan, Lei Zhao, Dalong Zhang, Lixia Chen</details>
[![Paper](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2404.11474)
[![Code](https://img.shields.io/github/stars/Jamie-Cheung/LSAST.svg?style=social&label=Star)](https://github.com/Jamie-Cheung/LSAST)

+ **Customizing Text-to-Image Models with a Single Image Pair** (2 May 2024) <details><summary>[SIGGRAPH Asia 2024] Maxwell Jones et al.</summary>Maxwell Jones, Sheng-Yu Wang, Nupur Kumari, David Bau, Jun-Yan Zhu</details>
[![Paper](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2405.01536)
[![Code](https://img.shields.io/github/stars/PairCustomization/PairCustomization.svg?style=social&label=Star)](https://github.com/PairCustomization/PairCustomization)
[![Page](https://img.shields.io/badge/Page-green)](https://paircustomization.github.io/)

+ **InstantStyle-Plus: Style Transfer with Content-Preserving in Text-to-Image Generation** (30 Jun 2024) <details><summary>Haofan Wang, Peng Xing et al.</summary>Haofan Wang, Peng Xing, Renyuan Huang, Hao Ai, Qixun Wang, Xu Bai</details>
[![Paper](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2407.00788)
[![Code](https://img.shields.io/github/stars/instantX-research/InstantStyle-Plus.svg?style=social&label=Star)](https://github.com/instantX-research/InstantStyle-Plus)
[![Page](https://img.shields.io/badge/Page-green)](https://instantstyle-plus.github.io/)

+ **D2Styler: Advancing Arbitrary Style Transfer with Discrete Diffusion Methods** (7 Aug 2024) <details><summary>[ICPR 2024] Onkar Susladkar, Gayatri Deshmukh et al.</summary>Onkar Susladkar, Gayatri Deshmukh, Sparsh Mittal, Parth Shastri</details>
[![Paper](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2408.03558)
[![Code](https://img.shields.io/github/stars/Onkarsus13/D2Styler.svg?style=social&label=Star)](https://github.com/Onkarsus13/D2Styler)

+ **Single Trajectory Distillation for Accelerating Image and Video Style Transfer** (25 Dec 2024) <details><summary>Sijie Xu, Runqi Wang et al.</summary>Sijie Xu, Runqi Wang, Wei Zhu, Dejia Song, Nemo Chen, Xu Tang, Yao Hu</details>
[![Paper](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2412.18945v1)
[![Page](https://img.shields.io/badge/Page-green)]([![Page](https://img.shields.io/badge/Page-green)](https://paircustomization.github.io/))

+ **StyleRWKV: High-Quality and High-Efficiency Style Transfer with RWKV-like Architecture** (27 Dec 2024) <details><summary>Miaomiao Dai, Qianyu Zhou et al.</summary>Miaomiao Dai, Qianyu Zhou, Lizhuang Ma</details>
[![Paper](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2412.19535)

+ **StyleSSP: Sampling StartPoint Enhancement for Training-free Diffusion-based Method for Style Transfer** (20 Jan 2025) <details><summary>[CVPR 2025] Ruojun Xu, Weijie Xi et al.</summary>Ruojun Xu, Weijie Xi, Xiaodi Wang, Yongbo Mao, Zach Cheng</details>
[![Paper](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2501.11319)
[![Code](https://img.shields.io/github/stars/bytedance/StyleSSP.svg?style=social&label=Star)](https://github.com/bytedance/StyleSSP)

+ **AttenST: A Training-Free Attention-Driven Style Transfer Framework with Pre-Trained Diffusion Models** (10 Mar 2025) <details><summary>Bo Huang et al.</summary>Bo Huang, Wenlun Xu, Qizhuo Han, Haodong Jing, Ying Li</details>
[![Paper](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2503.07307)
[![Code](https://img.shields.io/github/stars/HuanBor/AttenST.svg?style=social&label=Star)](https://github.com/HuanBor/AttenST)

+ **SEMANTIX: AN ENERGY-GUIDED SAMPLER FOR SEMANTIC STYLE TRANSFER** (28 Mar 2025) <details><summary>[ICLR 2025] Huiang He et al.</summary>Huiang He, Minghui Hu, Chuanxia Zheng, Chaoyue Wang, Tat-Jen Cham</details>
[![Paper](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2503.22344)

### None Diffusion Models
+ **Aesthetic-aware image style transfer.** <details><summary>[MM 2020] Zhiyuan Hu, Jia Jia et al.</summary>Zhiyuan Hu, Jia Jia, Bei Liu, Yaohua Bu and Jianlong Fu</details>
[![Paper](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://hcsi.cs.tsinghua.edu.cn/Paper/Paper20/MM20-HUZHIYUAN.pdf)
[![Code](https://img.shields.io/github/stars/researchmm/AAST-pytorch.svg?style=social&label=Star)](https://github.com/researchmm/AAST-pytorch)

+ **AdaAttN: Revisit Attention Mechanism in Arbitrary Neural Style Transfer** (8 Aug 2021) <details><summary>[ICCV 2021] Songhua Liu, Tianwei Lin et al.</summary>Songhua Liu, Tianwei Lin, Dongliang He, Fu Li, Meiling Wang, Xin Li, Zhengxing Sun, Qian Li, Errui Ding</details>
[![Paper](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2108.03647)
[![Code](https://img.shields.io/github/stars/Huage001/AdaAttN.svg?style=social&label=Star)](https://github.com/Huage001/AdaAttN)

+ **Artistic Style Transfer with Internal-external Learning and Contrastive Learning** <details><summary>[NeurIPS 2021] Haibo Chen, Lei Zhao et al.</summary>Haibo Chen, Lei Zhao, Zhizhong Wang, Huiming Zhang, Zhiwen Zuo, Ailin Li, Wei Xing, Dongming Lu</details>
[![Paper](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://proceedings.neurips.cc/paper/2021/file/df5354693177e83e8ba089e94b7b6b55-Paper.pdf)
[![Code](https://img.shields.io/github/stars/HalbertCH/IEContraAST.svg?style=social&label=Star)](https://github.com/HalbertCH/IEContraAST) 

+ **Exact Feature Distribution Matching for Arbitrary Style Transfer and Domain Generalization** (15 Mar 2022) <details><summary>[CVPR 2022] Yabin Zhang, Minghan Li et al.</summary>Yabin Zhang, Minghan Li, Ruihuang Li, Kui Jia, Lei Zhang</details>
[![Paper](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2203.07740)
[![Code](https://img.shields.io/github/stars/YBZh/EFDM.svg?style=social&label=Star)](https://github.com/YBZh/EFDM) 

+ **Unpaired Cartoon Image Synthesis via Gated Cycle Mapping** <details><summary>[CVPR 2022] Yifang Men, Yuan Yao et al.</summary>Yifang Men, Yuan Yao, Miaomiao Cui, Zhouhui Lian, Xuansong Xie, Xian-Sheng Hua</details>
[![Paper](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://openaccess.thecvf.com/content/CVPR2022/papers/Men_Unpaired_Cartoon_Image_Synthesis_via_Gated_Cycle_Mapping_CVPR_2022_paper.pdf)
[![Page](https://img.shields.io/badge/Page-green)](https://menyifang.github.io/projects/UCIS/UCIS.html)

+ **Artistic Style Discovery With Independent Components** <details><summary>[CVPR 2022] Xin Xie, Yi Li et al.</summary>Xin Xie, Yi Li, Huaibo Huang, Haiyan Fu, Wanwan Wang, Yanqing Guo</details>
[![Paper](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://openaccess.thecvf.com/content/CVPR2022/papers/Xie_Artistic_Style_Discovery_With_Independent_Components_CVPR_2022_paper.pdf)
[![Code](https://img.shields.io/github/stars/Shelsin/ArtIns.svg?style=social&label=Star)](https://github.com/Shelsin/ArtIns) 

+ **MicroAST: Towards Super-Fast Ultra-Resolution Arbitrary Style Transfer** (28 Nov 2022) <details><summary>[AAAI 2023] Zhizhong Wang, Lei Zhao et al.</summary>Zhizhong Wang, Lei Zhao, Zhiwen Zuo, Ailin Li, Haibo Chen, Wei Xing, Dongming Lu</details>
[![Paper](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2211.15313)
[![Code](https://img.shields.io/github/stars/EndyWon/MicroAST.svg?style=social&label=Star)](https://github.com/EndyWon/MicroAST) 

+ **QuantArt: Quantizing Image Style Transfer Towards High Visual Fidelity** (20 Dec 2022) <details><summary>[CVPR 2023] Siyu Huang, Jie An et al.</summary>Siyu Huang, Jie An, Donglai Wei, Jiebo Luo, Hanspeter Pfister</details>
[![Paper](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2212.10431)
[![Code](https://img.shields.io/github/stars/siyuhuang/QuantArt.svg?style=social&label=Star)](https://github.com/siyuhuang/QuantArt) 

+ **All-to-key Attention for Arbitrary Style Transfer** (8 Dec 2022) <details><summary>[ICCV 2023] Mingrui Zhu, Xiao He et al.</summary>Mingrui Zhu, Xiao He, Nannan Wang, Xiaoyu Wang, Xinbo Gao</details>
[![Paper](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2212.04105)
[![Code](https://img.shields.io/github/stars/LearningHx/StyA2K.svg?style=social&label=Star)](https://github.com/LearningHx/StyA2K) 

+ **StylerDALLE: Language-Guided Style Transfer Using a Vector-Quantized Tokenizer of a Large-Scale Generative Model** (16 Mar 2023) <details><summary>[ICCV 2023] Zipeng Xu, Enver Sangineto et al.</summary>Zipeng Xu, Enver Sangineto, Nicu Sebe</details>
[![Paper](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2303.09268)
[![Code](https://img.shields.io/github/stars/zipengxuc/StylerDALLE.svg?style=social&label=Star)](https://github.com/zipengxuc/StylerDALLE) 

+ **AesPA-Net: Aesthetic Pattern-Aware Style Transfer Networks** (19 Jul 2023) <details><summary>[ICCV 2023] Kibeom Hong, Seogkyu Jeon et al.</summary>Kibeom Hong, Seogkyu Jeon, Junsoo Lee, Namhyuk Ahn, Kunhee Kim, Pilhyeon Lee, Daesik Kim, Youngjung Uh, Hyeran Byun</details>
[![Paper](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2307.09724)
[![Code](https://img.shields.io/github/stars/Kibeom-Hong/AesPA-Net.svg?style=social&label=Star)](https://github.com/Kibeom-Hong/AesPA-Net) 

+ **Learning Dynamic Style Kernels for Artistic Style Transfer** <details><summary>[CVPR 2023] Wenju Xu, Chengjiang Long et al.</summary>Wenju Xu, Chengjiang Long, Yongwei Nie</details>
[![Paper](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://openaccess.thecvf.com/content/CVPR2023/papers/Xu_Learning_Dynamic_Style_Kernels_for_Artistic_Style_Transfer_CVPR_2023_paper.pdf)

+ **Dual-head Genre-instance Transformer Network for Arbitrary Style Transfer** <details><summary>[MM 2024] Meichen Liu, Shuting He et al.</summary>Meichen Liu, Shuting He, Songnan Lin, Bihan Wen</details>
[![Paper](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://dl.acm.org/doi/10.1145/3664647.3681569)

+ **A Training-Free Style-aligned Image Generation  with Scale-wise Autoregressive Model** (8 Apr 2025) <details><summary>Jihun Park et al.</summary>Jihun Park, Jongmin Gim, Kyoungmin Lee, Minseok Oh, Minwoo Choi, Jaeyeul Kim, Woo Chool Park, Sunghoon Im</details>
[![Paper](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2504.06144)

### Text-Guided Style Transfer

+ **DiffStyler: Controllable Dual Diffusion for Text-Driven Image Stylization** (19 Nov 2022) <details><summary>Nisha Huang, Yuxin Zhang et al.</summary>Nisha Huang, Yuxin Zhang, Fan Tang, Chongyang Ma, Haibin Huang, Yong Zhang, Weiming Dong, Changsheng Xu</details>
[![Paper](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2211.10682)
[![Code](https://img.shields.io/github/stars/haha-lisa/Diffstyler.svg?style=social&label=Star)](https://github.com/haha-lisa/Diffstyler) 

+ **Zero-Shot Contrastive Loss for Text-Guided Diffusion Image Style Transfer** (15 Mar 2023) <details><summary>[ICCV 2023] Serin Yang , Hyunmin Hwang et al.</summary>Serin Yang , Hyunmin Hwang, Jong Chul Ye</details>
[![Paper](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/pdf/2303.08622)

+ **StyleBooth: Image Style Editing with Multimodal Instruction** (18 Apr 2024) <details><summary>Zhen Han, Chaojie Mao et al.</summary>Zhen Han, Chaojie Mao, Zeyinzi Jiang, Yulin Pan, Jingfeng Zhang</details>
[![Paper](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2404.12154)
[![Code](https://img.shields.io/github/stars/modelscope/scepter.svg?style=social&label=Star)](https://github.com/modelscope/scepter) 
[![Page](https://img.shields.io/badge/Page-green)](https://ali-vilab.github.io/stylebooth-page/)

# 📍 Video Synthesis
## Text-to-Video Generation

+ **Style-A-Video: Agile Diffusion for Arbitrary Text-based Video Style Transfer** (9 May 2023) <details><summary>[IEEE Signal Processing Letters] Nisha Huang, Yuxin Zhang et al.</summary>Nisha Huang, Yuxin Zhang, Weiming Dong</details>
[![Paper](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2305.05464)

+ **StyleCrafter: Enhancing Stylized Text-to-Video Generation with Style Adapter** (1 Dec 2023) <details><summary>[SIGGRAPH Asia 2024 (Journal Track)] Gongye Liu, Menghan Xia et al.</summary>Gongye Liu, Menghan Xia, Yong Zhang, Haoxin Chen, Jinbo Xing, Yibo Wang, Xintao Wang, Yujiu Yang, Ying Shan</details>
[![Paper](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2312.00330)
[![Code](https://img.shields.io/github/stars/GongyeLiu/StyleCrafter.svg?style=social&label=Star)](https://github.com/GongyeLiu/StyleCrafter) 
[![Page](https://img.shields.io/badge/Page-green)](https://gongyeliu.github.io/StyleCrafter.github.io/)

+ **StyleMaster: Stylize Your Video with Artistic Generation and Translation** (10 Dec 2024) <details><summary>Zixuan Ye, Huijuan Huang et al.</summary>Zixuan Ye, Huijuan Huang, Xintao Wang, Pengfei Wan, Di Zhang, Wenhan Luo</details>
[![Paper](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2412.07744)
[![Code](https://img.shields.io/github/stars/KwaiVGI/StyleMaster.svg?style=social&label=Star)](https://github.com/KwaiVGI/StyleMaster) 
[![Page](https://img.shields.io/badge/Page-green)](https://zixuan-ye.github.io/stylemaster/)

## Video-to-Video Translation
+ **Rerender A Video: Zero-Shot Text-Guided Video-to-Video Translation** (13 Jun 2023) <details><summary>[SIGGRAPH Asia 2023] Shuai Yang, Yifan Zhou et al.</summary>Shuai Yang, Yifan Zhou, Ziwei Liu, Chen Change Loy</details>
[![Paper](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2306.07954)
[![Code](https://img.shields.io/github/stars/williamyang1991/Rerender_A_Video.svg?style=social&label=Star)](https://github.com/williamyang1991/Rerender_A_Video) 
[![Page](https://img.shields.io/badge/Page-green)](https://www.mmlab-ntu.com/project/rerender/)

+ **Pix2Video: Video Editing using Image Diffusion** (22 Mar 2023) <details><summary>[ICCV 2023] Duygu Ceylan et al.</summary>Duygu Ceylan, Chun-Hao Paul Huang, Niloy J. Mitra</details>
[![Paper](https://img.shields.io/badge/arXiv-b31b1b.svg)]()
[![Code](https://img.shields.io/github/stars/duyguceylan/pix2video.svg?style=social&label=Star)](https://github.com/duyguceylan/pix2video) 
[![Page](https://img.shields.io/badge/Page-green)](https://duyguceylan.github.io/pix2video.github.io/)

+ **FateZero: Fusing Attentions for Zero-shot Text-based Video Editing** (16 Mar 2023) <details><summary>[ICCV 2023] Chenyang Qi, Xiaodong Cun et al.</summary>Chenyang Qi, Xiaodong Cun, Yong Zhang, Chenyang Lei, Xintao Wang, Ying Shan, Qifeng Chen</details>
[![Paper](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2303.09535)
[![Code](https://img.shields.io/github/stars/ChenyangQiQi/FateZero.svg?style=social&label=Star)](https://github.com/ChenyangQiQi/FateZero) 
[![Page](https://img.shields.io/badge/Page-green)](https://fate-zero-edit.github.io/)

+ **FastBlend: a Powerful Model-Free Toolkit Making Video Stylization Easier** (15 Nov 2023) <details><summary>Zhongjie Duan, Chengyu Wang et al.</summary>Zhongjie Duan, Chengyu Wang, Cen Chen, Weining Qian, Jun Huang, Mingyi Jin</details>
[![Paper](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2311.09265)
[![Code](https://img.shields.io/github/stars/Artiprocher/sd-webui-fastblend.svg?style=social&label=Star)](https://github.com/Artiprocher/sd-webui-fastblend) 

+ **Diffutoon: High-Resolution Editable Toon Shading via Diffusion Models** (29 Jan 2024) <details><summary>[IJCAI 2024] Zhongjie Duan, Chengyu Wang et al.</summary>Zhongjie Duan, Chengyu Wang, Cen Chen, Weining Qian, Jun Huang</details>
[![Paper](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2401.16224)
[![Code](https://img.shields.io/github/stars/modelscope/DiffSynth-Studio.svg?style=social&label=Star)](https://github.com/modelscope/DiffSynth-Studio) 
[![Page](https://img.shields.io/badge/Page-green)](https://ecnu-cilab.github.io/DiffutoonProjectPage/)


+ **Customize-A-Video: One-Shot Motion Customization of Text-to-Video Diffusion Models** (22 Feb 2024) <details><summary>[ECCV 2024] Yixuan Ren, Yang Zhou et al.</summary>Yixuan Ren, Yang Zhou, Jimei Yang, Jing Shi, Difan Liu, Feng Liu, Mingi Kwon, Abhinav Shrivastava</details>
[![Paper](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2402.14780)
[![Page](https://img.shields.io/badge/Page-green)](https://ryx19th.github.io/customize-a-video/)

+ **Looking Backward: Streaming Video-to-Video Translation with Feature Banks** (24 May 2024) <details><summary>Feng Liang, Akio Kodaira et al.</summary>Feng Liang, Akio Kodaira, Chenfeng Xu, Masayoshi Tomizuka, Kurt Keutzer, Diana Marculescu</details>
[![Paper](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2405.15757)
[![Code](https://img.shields.io/github/stars/Jeff-LiangF/streamv2v.svg?style=social&label=Star)](https://github.com/Jeff-LiangF/streamv2v) 
[![Page](https://img.shields.io/badge/Page-green)](https://jeff-liangf.github.io/projects/streamv2v/)

+ **AniDoc: Animation Creation Made Easier** (18 Dec 2024) <details><summary>Yihao Meng, Hao Ouyang et al.</summary>Yihao Meng, Hao Ouyang, Hanlin Wang, Qiuyu Wang, Wen Wang, Ka Leong Cheng, Zhiheng Liu, Yujun Shen, Huamin Qu</details>
[![Paper](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2412.14173)
[![Code](https://img.shields.io/github/stars/yihao-meng/AniDoc.svg?style=social&label=Star)](https://github.com/yihao-meng/AniDoc) 
[![Page](https://img.shields.io/badge/Page-green)](https://yihao-meng.github.io/AniDoc_demo/)


# 📍 3D Generation

+ **TEXTure: Text-Guided Texturing of 3D Shapes** (3 Feb 2023) <details><summary>[SIGGRAPH 2023] Elad Richardson, Gal Metzer et al.</summary>Elad Richardson, Gal Metzer, Yuval Alaluf, Raja Giryes, Daniel Cohen-Or</details>
[![Paper](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2302.01721)
[![Code](https://img.shields.io/github/stars/TEXTurePaper/TEXTurePaper.svg?style=social&label=Star)](https://github.com/TEXTurePaper/TEXTurePaper) 
[![Page](https://img.shields.io/badge/Page-green)](https://texturepaper.github.io/TEXTurePaper/)

+ **Paint-it: Text-to-Texture Synthesis via Deep Convolutional Texture Map Optimization and Physically-Based Rendering** (18 Dec 2023) <details><summary>[CVPR 2024] Kim Youwang et al.</summary>Kim Youwang, Tae-Hyun Oh, Gerard Pons-Moll</details>
[![Paper](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2312.11360)
[![Code](https://img.shields.io/github/stars/postech-ami/paint-it.svg?style=social&label=Star)](https://github.com/postech-ami/paint-it) 
[![Page](https://img.shields.io/badge/Page-green)](https://kim-youwang.github.io/paint-it)

+ **TextureDreamer: Image-guided Texture Synthesis through Geometry-aware Diffusion** (17 Jan 2024) <details><summary>[CVPR 2024] Yu-Ying Yeh, Jia-Bin Huang et al.</summary>Yu-Ying Yeh, Jia-Bin Huang, Changil Kim, Lei Xiao, Thu Nguyen-Phuoc, Numair Khan, Cheng Zhang, Manmohan Chandraker, Carl S Marshall, Zhao Dong, Zhengqin Li</details>
[![Paper](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2401.09416)
[![Page](https://img.shields.io/badge/Page-green)](https://texturedreamer.github.io/)

+ **StyleTex: Style Image-Guided Texture Generation for 3D Models** (1 Nov 2024) <details><summary>[SIGGRAPH Asia 2024] Zhiyu Xie, Yuqing Zhang et al.</summary>Zhiyu Xie, Yuqing Zhang, Xiangjun Tang, Yiqian Wu, Dehan Chen, Gongsheng Li, Xaogang Jin</details>
[![Paper](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2411.00399)

+ **Style3D: Attention-guided Multi-view Style Transfer for 3D Object Generation** (4 Dec 2024) <details><summary>Bingjie Song, Xin Huang et al.</summary>Bingjie Song, Xin Huang, Ruting Xie, Xue Wang, Qing Wang</details>
[![Paper](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2412.03571)


# 📍 Related Research and Surveys
+ **Image Style Transfer Using Convolutional Neural Networks** <details><summary>[CVPR 2016] Leon A. Gatys et al.</summary>Leon A. Gatys, Alexander S. Ecker, Matthias Bethge</details>
[![Paper](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://www.cv-foundation.org/openaccess/content_cvpr_2016/papers/Gatys_Image_Style_Transfer_CVPR_2016_paper.pdf)
[![Code](https://img.shields.io/github/stars/superb20/Image-Style-Transfer-Using-Convolutional-Neural-Networks.svg?style=social&label=Star)](https://github.com/superb20/Image-Style-Transfer-Using-Convolutional-Neural-Networks) 

+ **StyleBank: An Explicit Representation for Neural Image Style Transfer** (27 Mar 2017) <details><summary>[CVPR 2017] Dongdong Chen, Lu Yuan et al.</summary>Dongdong Chen, Lu Yuan, Jing Liao, Nenghai Yu, Gang Hua</details>
[![Paper](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/1703.09210)

+ **StyleCLIPDraw: Coupling Content and Style in Text-to-Drawing Translation** (24 Feb 2022) <details><summary>[IJCAI 2022] Peter Schaldenbrand, Zhixuan Liu et al.</summary>Peter Schaldenbrand, Zhixuan Liu, Jean Oh</details>
[![Paper](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2202.12362)

+ **Simple Disentanglement of Style and Content in Visual Representations** (20 Feb 2023) <details><summary>[ICML 2023] Lilian Ngweta, Subha Maity et al.</summary>Lilian Ngweta, Subha Maity, Alex Gittens, Yuekai Sun, Mikhail Yurochkin</details>
[![Paper](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2302.09795)
[![Code](https://img.shields.io/github/stars/lilianngweta/PISCO.svg?style=social&label=Star)](https://github.com/lilianngweta/PISCO) 

+ **Text2Video-Zero: Text-to-Image Diffusion Models are Zero-Shot Video Generators** (23 Mar 2023) <details><summary>[ICCV 2023] Levon Khachatryan et al.</summary>Levon Khachatryan, Andranik Movsisyan, Vahram Tadevosyan, Roberto Henschel, Zhangyang Wang, Shant Navasardyan, Humphrey Shi</details>
[![Paper](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2303.13439)
[![Code](https://img.shields.io/github/stars/Picsart-AI-Research/Text2Video-Zero.svg?style=social&label=Star)](https://github.com/Picsart-AI-Research/Text2Video-Zero) 
[![Page](https://img.shields.io/badge/Page-green)](https://text2video-zero.github.io/)

+ **VideoComposer: Compositional Video Synthesis with Motion Controllability** (3 Jun 2023) <details><summary>[ICCV 2023] Xiang Wang et al.</summary>Xiang Wang, Hangjie Yuan, Shiwei Zhang, Dayou Chen, Jiuniu Wang, Yingya Zhang, Yujun Shen, Deli Zhao, Jingren Zhou</details>
[![Paper](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2306.02018)
[![Code](https://img.shields.io/github/stars/ali-vilab/videocomposer.svg?style=social&label=Star)](https://github.com/ali-vilab/videocomposer) 
[![Page](https://img.shields.io/badge/Page-green)](https://videocomposer.github.io/)

+ **UnlearnCanvas: A Stylized Image Dataset to Benchmark Machine Unlearning for Diffusion Models** (19 Feb 2024) <details><summary>[NeurIPS 2024 D&B Track] Yihua Zhang et al.</summary>Yihua Zhang, Chongyu Fan, Yimeng Zhang, Yuguang Yao, Jinghan Jia, Jiancheng Liu, Gaoyuan Zhang, Gaowen Liu, Ramana Rao Kompella, Xiaoming Liu, Sijia Liu</details>
[![Paper](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2402.11846)
[![Code](https://img.shields.io/github/stars/OPTML-Group/UnlearnCanvas.svg?style=social&label=Star)](https://github.com/OPTML-Group/UnlearnCanvas) 

+ **Diffusion Model-Based Image Editing: A Survey** (27 Feb 2024) <details><summary>Yi Huang et al.</summary>Yi Huang, Jiancheng Huang, Yifan Liu, Mingfu Yan, Jiaxi Lv, Jianzhuang Liu, Wei Xiong, He Zhang, Shifeng Chen, Liangliang Cao</details>
[![Paper](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2402.17525)

+ **Conditional Image Synthesis with Diffusion Models: A Survey** (28 Sep 2024) <details><summary>Bingyuan Wang et al.</summary>Bingyuan Wang, Qifeng Chen, Zeyu Wang</details>
[![Paper](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2408.12128)

+ **Conditional Image Synthesis with Diffusion Models: A Survey** (28 Sep 2024) <details><summary>Zheyuan Zhan et al.</summary>Zheyuan Zhan, Defang Chen, Jian-Ping Mei, Zhenghe Zhao, Jiawei Chen, Chun Chen, Siwei Lyu, Can Wang</details>
[![Paper](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2409.19365)
[![Code](https://img.shields.io/github/stars/zju-pi/Awesome-Conditional-Diffusion-Models.svg?style=social&label=Star)](https://github.com/zju-pi/Awesome-Conditional-Diffusion-Models) 