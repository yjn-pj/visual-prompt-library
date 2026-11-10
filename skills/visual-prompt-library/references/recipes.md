# 案例索引和模板

| 用途 | YouMind 视觉线索 | ZeroLu 结构线索 | 改编字段 |
| --- | --- | --- | --- |
| 手绘封面 | [从照片做手绘头图](https://github.com/YouMind-OpenLab/awesome-nano-banana-pro-prompts/blob/c2f26af1683e8c9bd9b1ffc9f2b9ed978dbf1601/README.md#no-3-hand-drawn-style-header-image-prompt-from-photo) | [电影关键帧](https://github.com/ZeroLu/awesome-nanobanana-pro/blob/83fab46434881d0e86544a6b9820085078a3aaf6/README.md#216-cinematic-keyframe-generator) | 主体轮廓、场景、景别、手绘媒介、主色、标题留白 |
| 商品棚拍 | [电商静物广告](https://github.com/YouMind-OpenLab/awesome-nano-banana-pro-prompts/blob/c2f26af1683e8c9bd9b1ffc9f2b9ed978dbf1601/README.md#no-108-e-commerce-main-image---luxury-chocolate-ad-still-life) | [奢侈品摄影](https://github.com/ZeroLu/awesome-nanobanana-pro/blob/83fab46434881d0e86544a6b9820085078a3aaf6/README.md#117-luxury-product-photography)、[专业商品摄影](https://github.com/ZeroLu/awesome-nanobanana-pro/blob/83fab46434881d0e86544a6b9820085078a3aaf6/README.md#42-professional-product-photography) | 产品比例、表面纹理、承托面、相机角度、主光方向、背景和反光 |
| 卖点信息图 | [液态玻璃 Bento](https://github.com/YouMind-OpenLab/awesome-nano-banana-pro-prompts/blob/c2f26af1683e8c9bd9b1ffc9f2b9ed978dbf1601/README.md#no-2-premium-liquid-glass-bento-grid-product-infographic-with-8-modules) | [概念信息图](https://github.com/ZeroLu/awesome-nanobanana-pro/blob/83fab46434881d0e86544a6b9820085078a3aaf6/README.md#31-concept-visualization-text-to-infographic) | 主卡、卖点顺序、每卡的图形和短标签、网格、文字原文 |
| 短剧关键帧 | [YouMind 中文索引](https://github.com/YouMind-OpenLab/awesome-nano-banana-pro-prompts/blob/main/README_zh.md) | [电影关键帧](https://github.com/ZeroLu/awesome-nanobanana-pro/blob/83fab46434881d0e86544a6b9820085078a3aaf6/README.md#216-cinematic-keyframe-generator) | 角色或道具的稳定特征、地点、当前动作、相机角度、单帧信息 |

## 画面约束

- 手绘封面先确定标题区域。用低对比背景托住标题区，再把主体和明暗反差集中在另一边。若会裁切，给主体突出的部位（例如提手）留出裁切余量。
- 棚拍先锁比例、零件和材质，再写灯光。用户有真实商品图时，用它作为造型依据。
- 信息图优先用少量大字号的精确短标签。每张卡只承载一个卖点。参数只采用用户给定或已核验的数据。需要整段文字时，将文案和画面底图分开。
- 关键帧每次出一张。参考案例有多格时，先选定其中一个镜头，再说明它必须交代的动作或情绪。

## GPT 图片 brief

写明画幅与用途，描述主体及必须保持的特征，接着写场景、媒介、构图、光线和材质。最后写标题区、逐字标签及对应位置。需要同一产品跨图复用时，用已经通过检查的成图作为主体参考，并在新 brief 中重申关键外观。
