# Computer Vision Notes

## Intro
### Human Visual System
*modality: 模态*。 视觉是一种模态

人类的视觉系统包括：

- Eyes (sensory organ)
- Parts of the central nervous system
    - Retina layers
    - Optic nerve
    - Optic tract
    - Visual cortex

Visual pathway: visual field->retina->optic nerve->...->optic tract->...->visual cortex

Visual System要做的事情：

- visual sensation（感受）

    Monocular Vision VS Binocular Vision and Stereopsis

    双眼可以感知立体视觉，对距离和方位存在disparity.

- visual perception（感知）：the process of acquiring knowledge about environmental objects and events by extracting information from the light they emit or reflect.

    视觉区别于相机的一点在于相机没有感知能力。

    examples: motion perception, pattern recognition(facial recognition), visual cognition.

- visual motor coordination（视觉运动协调）
    
    examples: Eye-Hand Coordination, Running, Balancing.

    Perception-Action Loop: 感知动作循环，定义高级智能（具身智能）

    interaction with language system

### History
- Low-level Vision: Processing and Feature Extaction. 防抖之类的最基本的操作。
- Mid-level Vision: make inferences about the world. 3D重建，扫地机器人，照片缝合等。 
- High-level Vision: Understand. 人脸识别，无人购物（最依赖深度学习）。

Graphics VS Vision: 逆过程。图形学是给定位置等还原画面（渲染 rendering）；计算机视觉是给定图片算位置。

Synthetic data: 用图形学来提供大量的数据集

embodied agents: 具身

大模型(LM): Disembodied Models（GPT-4v） + Embodies VLA Models（自驾）.

### Summary
Computer Vision **DO**:

- visual data acquisition (similar to human eyes but comes with many more choices)
- signal processing and feature extraction (mostly low-level)
- analyze local structures and then 3D reconstruct the original scene (midlevel)
- understanding (mostly high-level)
- generation
- vision-language tasks
- and further enabling embodied agents to take actions.