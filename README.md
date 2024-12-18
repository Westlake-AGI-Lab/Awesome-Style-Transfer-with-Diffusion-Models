<div align="center">
<h2> Awesome Style Transfer with Diffusion Models </h2> 
</div>

# 🤗 Introduction
- This repository contains a curated list of **Style Transfer with Diffusion Models**. The resources are organized into two main categories: Image Synthesis and Video Synthesis.

- We welcome any contributions and suggestions to our repository or the addition of your own work. Feel free to make a pull request or leave your comments!!

# 📋 Contents
- [🤗 Introduction](#-introduction)
- [📋 Contents](#-contents)
- [💘 Tips](#-tips)
- [📍 Image Synthesis](#-image-synthesis)
  - [Text-Driven Style Transfer](#text-driven-style-transfer)
    - [Image-Encoder Based](#image-encoder-based)
    - [Inversion-Based](#inversion-based)
    - [Swap Features In Attention Layer](#swap-features-in-attention-layer)
    - [Fine-tune Methods](#fine-tune-methods)
    - [Training-free Methods](#training-free-methods)
  - [Image-Driven Style Transfer](#image-driven-style-transfer)
    - [Text-Guided Style Transfer](#text-guided-style-transfer)
    - [None Diffusion Models](#none-diffusion-models)
- [📍 Video Synthesis](#-video-synthesis)
  - [Text-to-Video Generation](#text-to-video-generation)
  - [Video-to-Video Translation](#video-to-video-translation)
- [📍 Related Research](#-related-research)


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

+ **InstantStyle: Free Lunch towards Style-Preserving in Text-to-Image Generation** (3 Apr 2024) <details><summary>Haofan Wang, Matteo Spinelli et al.</summary>Haofan Wang, Matteo Spinelli, Qixun Wang, Xu Bai, Zekui Qin, Anthony Chen</details>
[![Paper](https://img.shields.io/badge/arXiv-b31b1b.svg)]()
[![Code](https://img.shields.io/github/stars/instantX-research/InstantStyle.svg?style=social&label=Star)](https://github.com/instantX-research/InstantStyle)
[![Page](https://img.shields.io/badge/Page-green)](https://instantstyle.github.io/)

+ **DEADiff: An Efficient Stylization Diffusion Model with Disentangled Representations** (11 Mar 2024) <details><summary>[CVPR 2024] Tianhao Qi, Shancheng Fang et al.</summary>Tianhao Qi, Shancheng Fang, Yanze Wu, Hongtao Xie, Jiawei Liu, Lang Chen, Qian He, Yongdong Zhang</details>
[![Paper](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2403.06951)
[![Code](https://img.shields.io/github/stars/bytedance/DEADiff.svg?style=social&label=Star)](https://github.com/bytedance/DEADiff)
[![Page](https://img.shields.io/badge/Page-green)](https://tianhao-qi.github.io/DEADiff/)

+ **ArtAdapter: Text-to-Image Style Transfer using Multi-Level Style Encoder and Explicit Adaptation** (4 Dec 2023) <details><summary>[CVPR 2024] Dar-Yen Chen, Hamish Tennent et al.</summary>Dar-Yen Chen, Hamish Tennent, Ching-Wen Hsu</details>
[![Paper](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2312.02109)
[![Code](https://img.shields.io/github/stars/cardinalblue/ArtAdapter.svg?style=social&label=Star)](https://github.com/cardinalblue/ArtAdapter)
[![Page](https://img.shields.io/badge/Page-green)](https://cardinalblue.github.io/artadapter.github.io/)

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

+ **StyleStudio: Text-Driven Style Transfer with Selective Control of Style Elements** (11 Dec 2024) <details><summary> Mingkun Lei, Xue Song et al.</summary>Mingkun Lei, Xue Song, Beier Zhu, Hao Wang, Chi Zhang</details>
[![Paper](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2412.08503)
[![Code](https://img.shields.io/github/stars/alipay/style-tokenizer.svg?style=social&label=Star)](https://github.com/Westlake-AGI-Lab/StyleStudio) 
[![Page](https://img.shields.io/badge/Page-green)](https://stylestudio-official.github.io/)

### Inversion-Based

+ **An Image is Worth One Word: Personalizing Text-to-Image Generation using Textual Inversion** (2 Aug 2022) <details><summary>[ICLR 2023] Rinon Gal, Yuval Alaluf et al.</summary>Rinon Gal, Yuval Alaluf, Yuval Atzmon, Or Patashnik, Amit H. Bermano, Gal Chechik, Daniel Cohen-Or</details>
[![Paper](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2208.01618)
[![Code](https://img.shields.io/github/stars/rinongal/textual_inversion.svg?style=social&label=Star)](https://github.com/rinongal/textual_inversion)
[![Page](https://img.shields.io/badge/Page-green)](https://textual-inversion.github.io/)

+ **Inversion-Based Style Transfer with Diffusion Models** (23 Nov 2022) <details><summary>[CVPR 2023] Yuxin Zhang, Nisha Huang et al.</summary>Yuxin Zhang, Nisha Huang, Fan Tang, Haibin Huang, Chongyang Ma, Weiming Dong, Changsheng Xu</details>
[![Paper](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2211.13203)
[![Code](https://img.shields.io/github/stars/zyxElsa/InST.svg?style=social&label=Star)](https://github.com/zyxElsa/InST)

### Swap Features In Attention Layer

+ **Cross-Image Attention for Zero-Shot Appearance Transfer** (6 Nov 2023) <details><summary>[SIGGRAPH 2024] Yuval Alaluf, Daniel Garibi et al.</summary>Yuval Alaluf, Daniel Garibi, Or Patashnik, Hadar Averbuch-Elor, Daniel Cohen-Or</details>
[![Paper](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2311.03335)
[![Code](https://img.shields.io/github/stars/garibida/cross-image-attention.svg?style=social&label=Star)](https://github.com/garibida/cross-image-attention)
[![Page](https://img.shields.io/badge/Page-green)](https://garibida.github.io/cross-image-attention/)

+ **Style Aligned Image Generation via Shared Attention** (4 Dec 2023) <details><summary>[CVPR 2024] Amir Hertz, Andrey Voynov et al.</summary>Amir Hertz, Andrey Voynov, Shlomi Fruchter, Daniel Cohen-Or</details>
[![Paper](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2312.02133)
[![Code](https://img.shields.io/github/stars/google/style-aligned/.svg?style=social&label=Star)](https://github.com/google/style-aligned/)
[![Page](https://img.shields.io/badge/Page-green)](https://style-aligned-gen.github.io/)

+ **Visual Style Prompting with Swapping Self-Attention** (20 Feb 2024) <details><summary>Jaeseok Jeong, Junho Kim et al.</summary>Jaeseok Jeong, Junho Kim, Yunjey Choi, Gayoung Lee, Youngjung Uh</details>
[![Paper](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2402.12974)
[![Code](https://img.shields.io/github/stars/naver-ai/Visual-Style-Prompting.svg?style=social&label=Star)](https://github.com/naver-ai/Visual-Style-Prompting)
[![Page](https://img.shields.io/badge/Page-green)](https://curryjung.github.io/VisualStylePrompt/)

+ **StyleGuide: Crafting visual style prompting with negative visual query guidance**  
[![Paper](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://openreview.net/pdf?id=618qfjvSt9)

### Fine-tune Methods

+ **Diffusion in Style** <details><summary>[ICCV 2023] Martin Nicolas Everaert, Marco Bocchio et al.</summary>Martin Nicolas Everaert, Marco Bocchio, Sami Arpa, Sabine Süsstrunk, Radhakrishna Achanta</details>
[![Paper](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://openaccess.thecvf.com/content/ICCV2023/papers/Everaert_Diffusion_in_Style_ICCV_2023_paper.pdf)
[![Page](https://img.shields.io/badge/Page-green)](https://ivrl.github.io/diffusion-in-style/)

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

### Training-free Methods
+ **FreeDoM: Training-Free Energy-Guided Conditional Diffusion Model** (17 Mar 2023) <details><summary>[ICCV 2023] Jiwen Yu, Yinhuai Wang et al.</summary>Jiwen Yu, Yinhuai Wang, Chen Zhao, Bernard Ghanem, Jian Zhang</details>
[![Paper](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2303.09833)
[![Code](https://img.shields.io/github/stars/vvictoryuki/FreeDoM.svg?style=social&label=Star)](https://github.com/vvictoryuki/FreeDoM)

+ **RB-Modulation: Training-Free Personalization of Diffusion Models using Stochastic Optimal Control** (27 May 2024) <details><summary>Litu Rout, Yujia Chen et al.</summary>Litu Rout, Yujia Chen, Nataniel Ruiz, Abhishek Kumar, Constantine Caramanis, Sanjay Shakkottai, Wen-Sheng Chu</details>
[![Paper](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2405.17401)
[![Code](https://img.shields.io/github/stars/google/RB-Modulation.svg?style=social&label=Star)](https://github.com/google/RB-Modulation)
[![Page](https://img.shields.io/badge/Page-green)](https://rb-modulation.github.io/)


## Image-Driven Style Transfer

+ **General Image-to-Image Translation with One-Shot Image Guidance** (20 Jul 2023) <details><summary>Bin Cheng, Zuhao Liu et al.</summary>Bin Cheng, Zuhao Liu, Yunbo Peng, Yue Lin</details>
[![Paper](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2307.14352)
[![Code](https://img.shields.io/github/stars/CrystalNeuro/visual-concept-translator.svg?style=social&label=Star)](https://github.com/CrystalNeuro/visual-concept-translator) 

+ **StyleDiffusion: Controllable Disentangled Style Transfer via Diffusion Models** (15 Aug 2023) <details><summary>[ICCV 2023] Zhizhong Wang, Lei Zhao et al.</summary>Zhizhong Wang, Lei Zhao, Wei Xing</details>
[![Paper](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2308.07863)

+ **Diffusion-Enhanced PatchMatch: A Framework for Arbitrary Style Transfer with Diffusion Models** <details><summary>[CVPR 2023] Mark Hamazaspyan, Shant Navasardyan</summary>Mark Hamazaspyan, Shant Navasardyan</details>
[![Paper](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://openaccess.thecvf.com/content/CVPR2023W/GCV/papers/Hamazaspyan_Diffusion-Enhanced_PatchMatch_A_Framework_for_Arbitrary_Style_Transfer_With_Diffusion_CVPRW_2023_paper.pdf)

+ **Style Injection in Diffusion: A Training-free Approach for Adapting Large-scale Diffusion Models for Style Transfer** (11 Dec 2023) <details><summary>[CVPR 2024] Jiwoo Chung, Sangeek Hyun et al.</summary>Jiwoo Chung, Sangeek Hyun, Jae-Pil Heo</details>
[![Paper](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2312.09008)
[![Code](https://img.shields.io/github/stars/jiwoogit/StyleID.svg?style=social&label=Star)](https://github.com/jiwoogit/StyleID)
[![Page](https://img.shields.io/badge/Page-green)](https://jiwoogit.github.io/StyleID_site/)

+ **HiCAST: Highly Customized Arbitrary Style Transfer with Adapter Enhanced Diffusion Models** (11 Jan 2024) <details><summary>Hanzhang Wang, Haoran Wang et al.</summary>Hanzhang Wang, Haoran Wang, Jinze Yang, Zhongrui Yu, Zeke Xie, Lei Tian, Xinyan Xiao, Junjun Jiang, Xianming Liu, Mingming Sun</details>
[![Paper](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2312.09008)
[![Code](https://img.shields.io/github/stars/wd1511/HiCAST.svg?style=social&label=Star)](https://github.com/wd1511/HiCAST)

+ **AesFA: An Aesthetic Feature-Aware Arbitrary Neural Style Transfer** (10 Dec 2023) <details><summary>[AAAI 2024] Joonwoo Kwon, Sooyoung Kim et al.</summary>Joonwoo Kwon, Sooyoung Kim, Yuewei Lin, Shinjae Yoo, Jiook Cha</details>
[![Paper](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2312.05928)
[![Code](https://img.shields.io/github/stars/Jamie-Cheung/ArtBank.svg?style=social&label=Star)](https://github.com/Jamie-Cheung/ArtBank)

+ **ArtBank: Artistic Style Transfer with Pre-trained Diffusion Model and Implicit Style Prompt Bank** (11 Dec 2023) <details><summary>[AAAI 2024] Zhanjie Zhang, Quanwei Zhang et al.</summary>Zhanjie Zhang, Quanwei Zhang, Guangyuan Li, Wei Xing, Lei Zhao, Jiakai Sun, Zehua Lan, Junsheng Luan, Yiling Huang, Huaizhong Lin</details>
[![Paper](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2312.09008)
[![Code](https://img.shields.io/github/stars/Jamie-Cheung/ArtBank.svg?style=social&label=Star)](https://github.com/Jamie-Cheung/ArtBank)

+ **InstantStyle-Plus: Style Transfer with Content-Preserving in Text-to-Image Generation** (30 Jun 2024) <details><summary>Haofan Wang, Peng Xing et al.</summary>Haofan Wang, Peng Xing, Renyuan Huang, Hao Ai, Qixun Wang, Xu Bai</details>
[![Paper](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2407.00788)
[![Code](https://img.shields.io/github/stars/instantX-research/InstantStyle-Plus.svg?style=social&label=Star)](https://github.com/instantX-research/InstantStyle-Plus)
[![Page](https://img.shields.io/badge/Page-green)](https://instantstyle-plus.github.io/)

+ **D2Styler: Advancing Arbitrary Style Transfer with Discrete Diffusion Methods** (7 Aug 2024) <details><summary>[ICPR 2024] Onkar Susladkar, Gayatri Deshmukh et al.</summary>Onkar Susladkar, Gayatri Deshmukh, Sparsh Mittal, Parth Shastri</details>
[![Paper](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2408.03558)
[![Code](https://img.shields.io/github/stars/Onkarsus13/D2Styler.svg?style=social&label=Star)](https://github.com/Onkarsus13/D2Styler)

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

### Text-Guided Style Transfer
+ **Zero-Shot Contrastive Loss for Text-Guided Diffusion Image Style Transfer** (15 Mar 2023) <details><summary>[ICCV 2023] Serin Yang , Hyunmin Hwang et al.</summary>Serin Yang , Hyunmin Hwang, Jong Chul Ye</details>
[![Paper](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/pdf/2303.08622)


# 📍 Video Synthesis
## Text-to-Video Generation

+ **StyleCrafter: Enhancing Stylized Text-to-Video Generation with Style Adapter** (1 Dec 2023) <details><summary>[SIGGRAPH Asia 2024 (Journal Track)] Gongye Liu, Menghan Xia et al.</summary>Gongye Liu, Menghan Xia, Yong Zhang, Haoxin Chen, Jinbo Xing, Yibo Wang, Xintao Wang, Yujiu Yang, Ying Shan</details>
[![Paper](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2312.00330)
[![Code](https://img.shields.io/github/stars/GongyeLiu/StyleCrafter.svg?style=social&label=Star)](https://github.com/GongyeLiu/StyleCrafter) 
[![Page](https://img.shields.io/badge/Page-green)](https://gongyeliu.github.io/StyleCrafter.github.io/)

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

+ **Looking Backward: Streaming Video-to-Video Translation with Feature Banks** (24 May 2024) <details><summary>Feng Liang, Akio Kodaira et al.</summary>Feng Liang, Akio Kodaira, Chenfeng Xu, Masayoshi Tomizuka, Kurt Keutzer, Diana Marculescu</details>
[![Paper](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2405.15757)
[![Code](https://img.shields.io/github/stars/Jeff-LiangF/streamv2v.svg?style=social&label=Star)](https://github.com/Jeff-LiangF/streamv2v) 
[![Page](https://img.shields.io/badge/Page-green)](https://jeff-liangf.github.io/projects/streamv2v/)

+ **StyleMaster: Stylize Your Video with Artistic Generation and Translation** () <details><summary></summary></details>
[![Paper](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2412.07744)
[![Code](https://img.shields.io/github/stars/KwaiVGI/StyleMaster.svg?style=social&label=Star)](https://github.com/KwaiVGI/StyleMaster) 
[![Page](https://img.shields.io/badge/Page-green)](https://zixuan-ye.github.io/stylemaster/)

+ **Customize-A-Video: One-Shot Motion Customization of Text-to-Video Diffusion Models** (22 Feb 2024) <details><summary>[ECCV 2024] Yixuan Ren, Yang Zhou et al.</summary>Yixuan Ren, Yang Zhou, Jimei Yang, Jing Shi, Difan Liu, Feng Liu, Mingi Kwon, Abhinav Shrivastava</details>
[![Paper](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2402.14780)
[![Page](https://img.shields.io/badge/Page-green)](https://ryx19th.github.io/customize-a-video/)

# 📍 Related Research
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