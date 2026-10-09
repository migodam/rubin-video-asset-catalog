# Rubin台本策划输入

目的：用已经完成的模型、静图和电影规划中文科普长视频。素材范围覆盖Vera Rubin NVL72、Vera CPU Rack、Groq 3 LPX、BlueField-4 STX/CMX、Spectrum-6 SPX/CPO五篇。

资料库：https://github.com/migodam/rubin-video-asset-catalog。更新时间：2026-10-10T02:56:18+08:00。

## 已有素材

- 67项自建模型：2个机房/跨尺度总装、5类机架、8类模块、8种PCB、8个芯片封装资产、3个存储/光学资产、33项原理模型。
- 201个三档主模型GLB，8个独立裸片示意GLB，以及分层Blender文件。
- 777张原生4K静图，包括六视角、接口、SOCAMM2压接、液冷、die逻辑分区、光学近景与6张Cycles关键静帧。
- 57组电影：114条3840×2160、30fps静默MP4，clean/annotated两版；合计642秒不同源镜头，重复两版不计成1284秒新内容。
- 78个独立讲解点、17条按问题选材的导航路线，以及一手技术来源。

公开目录中的预览已缩小；原始4K、Blender、GLB和MP4在本地完整包。文件名只用于台本素材引用，GPT网页浏览不能直接打开本地素材。

## 读哪些文件

1. [五篇选材](https://raw.githubusercontent.com/migodam/rubin-video-asset-catalog/main/ARTICLES.md)：主题主问题和现有镜头路线。
2. [57组镜头](https://raw.githubusercontent.com/migodam/rubin-video-asset-catalog/main/SHOTS.md)：ID、时长、阶段、帧号、秒数、时间轴预览。
3. [78个讲解点](https://raw.githubusercontent.com/migodam/rubin-video-asset-catalog/main/EXPLANATIONS.md)：要解释的机制、模型和镜头ID、近景、一手来源及边界。
4. [67个资产](https://raw.githubusercontent.com/migodam/rubin-video-asset-catalog/main/ASSETS.md) 与 [图册](https://github.com/migodam/rubin-video-asset-catalog/blob/main/GALLERY.md)：模型类别与可见内容。
5. [结构化完整目录](https://raw.githubusercontent.com/migodam/rubin-video-asset-catalog/main/data/catalog.json)：相同信息的机器可读版本。

## 重要限制

- 全部预览是自建模型或示意图；verified micrograph为0，不宣称厂商真实物理floorplan或制造级CAD。
- 机房40柜配比与建筑管线是展示布局：16 NVL72、12 LPX、8 SPX、2 Vera、2 STX。
- 6T/1T1C、TSV、光学、VRM与接头等为放大示意；不能按图估计真实制程尺寸、单元面积或器件性能。
- System-Level Cache与NAND Single-Level Cell是不同概念；原理文件分别建模。
- CPO发射端为ELS连续供光→EIC驱动→PIC调制；接收端为PD光电流→TIA电压→后续电处理。
- 集成III-V激光分支用于架构对照，不能改写成NVIDIA量产内部结构声明。
- 缓存、纠错、均衡、微环、负载与波形使用固定教学例子；没有逐周期RTL、电路、电光或瞬态数值仿真。
- Vera片内微字在部分角度低对比；15的标注版页脚另说明核心、SCF/L3、内存PHY和系统I/O。
- 55前段近俯视不能单独辨认chip→TIM→铜底纵向接触；使用功能剖面静图补充。
- 56的线圈会局部遮挡光点；57波形是归一化示例，不能当成量产实测曲线。
- 无独立正式SOCAMM2电影；SOCAMM2可用资产socamm2及07/09板级镜头与压接近景讲解。
- 全部57组源时间轴已实际采样；114片完整软件解码通过。完整连续视觉播放和用户审美批准未获得。

## 发给GPT的策划要求

请根据这份已完成的Rubin素材目录规划我的中文科普长视频台本。先读GPT_HANDOFF.md，再读SHOTS.md、EXPLANATIONS.md、ARTICLES.md；需要检查画面时再打开GALLERY.md和相关预览。

先给出一个能从机房讲到芯片、又能贯穿五类系统职责的主问题和章节安排，再给出逐段台本规划表：章节、观众需要解决的问题、旁白信息点、模型ID、镜头ID、具体阶段/源帧或可剪秒数、转场关系、静图/补充图形、技术来源、该画面不足以支持的结论。

尽量使用已存在的素材。允许重拍和延长现有模型镜头，但请标为“可用现有模型追加拍摄”；现成57组电影以SHOTS.md的时长与阶段为准。没有现成素材的内容请标“待补素材”，并说明为什么现有素材不够。

叙事先解释物理意义、工作场景和因果关系，再引入缩写与数值。避免堆规格、空泛宣传和重复整柜转场。五篇可以组织成一支连续长视频或系列篇章，先提出适合内容密度的时长分配，不把所有镜头强行用完，也不把642秒源镜头当成最终片长。

必须区分公开硬件外观重建、逻辑架构映射、放大教学示意、真实显微照片和实测数据。这里没有verified micrograph，也没有逐周期RTL、电光、电路或瞬态数值仿真。不得将System-Level Cache与NAND Single-Level Cell混淆，不得把III-V集成激光对照说成NVIDIA量产内部结构。对白中涉及实际芯片规格、产品版本和性能结论时，核验目录的一手来源；对话文章只决定主题范围。

先输出可审阅的完整结构与素材分配表，并指出影响台本的真实缺口，然后再写逐段旁白。
