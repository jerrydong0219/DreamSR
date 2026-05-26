<div align="center">
    <h1>PGP-DiffSR: Phase-Guided Progressive Pruning for Efficient Diffusion-based Image Super-Resolution</h1>
    <!-- <div>
        <a href='https://github.com/AnxQ/' target='_blank'>Xiaoqi An</a><sup>1</sup>&emsp;
        <a href='https://sharling-lz.github.io/' target='_blank'>Lin Zhao</a><sup>1</sup>&emsp;
        <a href='https://gcatnjust.github.io/ChenGong/index.html' target='_blank'>Chen Gong</a><sup>1</sup>&emsp;
        <a href='https://sites.google.com/view/junlineu/' target='_blank'>Jun Li</a><sup>1</sup>&emsp;
        <a href='https://scholar.google.com/citations?user=6CIDtZQAAAAJ&hl=zh-CN' target='_blank'>Jian Yang</a><sup>1</sup>
    </div> -->
    <!-- <div>
        <sup>School of Computer Science and Engineering, Nanjing University of Science and Technology
    </div> -->
</div>

<div align="center">
  
[![Paper](https://img.shields.io/badge/arXiv-PDF-b31b1b)](https://arxiv.org/abs/2605.15682)

</div>

Large-scale pre-trained diffusion models have been extensively adopted for real-world image Super-Resolution because of their powerful generative priors through textual guidance. However, when super-resolving high-resolution images with patch-wise inference strategy, most existing diffusion-based SR methods tend to suffer from over-generation, due to the misalignment between the global prompt from LR image and the incomplete semantic information of local patches during each inference step. On the other hand, most existing methods also failed to generate detailed texture in local patches due to the overemphasis on global generation capabilities in network designs and training strategies. To address this issue, we present DreamSR, a novel SR model that suppresses local over-generation and improves fine-detail synthesis, thereby achieving visually faithful results with ultra-high-quality details. Specifically, we propose a dual-branch MM-ControlNet, where the ControlNet generates local textual feature with patch-level prompts while the pre-trained DiT provides global textual feature with global prompts, thereby mitigating over-generation and ensuring semantic consistency across patches. We also design a comprehensive training strategy with stage-specific data processing pipelines and a Receptive-Field Enhancement strategy, enhancing the model's capability to capture patch information and effectively restore local textures. Extensive experiments demonstrate that DreamSR outperforms state-of-the-art methods, providing high-quality SR results.