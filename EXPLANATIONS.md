# Rubin现有78个讲解点

根据现有资产匹配讲解任务。文章章节只定位讨论题材；技术事实依据各条所列的一手资料核验。

## Vera Rubin NVL72

### assembly-hierarchy

POD→rack→tray→PCB层级与实体结构

要讲清楚：不透光壳体与可拆盖；导轨/锁扣/拉手/固定件；前后电/水/光接口分角色。

素材ID：`room`, `rack-nvl72`, `rack-vera`, `rack-lpx`, `rack-stx`, `rack-spx`, `tray-compute`, `tray-nvlink`, `tray-vera`, `tray-lpx`, `tray-stx`, `tray-etl`, `switch-sn6800`, `switch-sn6810`, `board-nvlink`, `board-etl`, `board-sn6800`, `board-sn6810`, `scene-pod-to-die`, `board-stx`。

镜头：[01-pod-tour](SHOTS.md#01-pod-tour), [02-rack-nvl72](SHOTS.md#02-rack-nvl72), [03-rack-vera](SHOTS.md#03-rack-vera), [04-rack-lpx](SHOTS.md#04-rack-lpx), [05-rack-stx](SHOTS.md#05-rack-stx), [06-rack-spx](SHOTS.md#06-rack-spx), [07-tray-compute](SHOTS.md#07-tray-compute), [08-tray-nvlink](SHOTS.md#08-tray-nvlink), [09-tray-vera](SHOTS.md#09-tray-vera), [10-tray-lpx](SHOTS.md#10-tray-lpx), [11-tray-stx](SHOTS.md#11-tray-stx), [12-tray-etl](SHOTS.md#12-tray-etl), [13-switch-sn6800](SHOTS.md#13-switch-sn6800), [14-switch-sn6810](SHOTS.md#14-switch-sn6810), [24-pod-to-die](SHOTS.md#24-pod-to-die)。

原章节：nvl72:01, vera:01-02, lpx:01-02, stx:02-03, spx:01。

近景：[assembled-detail](previews/room/assembled-detail.jpg) · [service-detail](previews/room/service-detail.jpg) · [pcb-detail](previews/room/pcb-detail.jpg)。

依据：[NVIDIA Vera Rubin POD: seven chips and five rack-scale systems](https://developer.nvidia.com/blog/nvidia-vera-rubin-pod-seven-chips-five-rack-scale-systems-one-ai-supercomputer/) · [DGX Vera Rubin NVL72 hardware guide](https://docs.nvidia.com/dgx/dgxvr-user-guide/hardware.html) · [NVIDIA Spectrum-6 SN6000 Switch Systems Hardware User Manual 1.3](https://networking-docs.nvidia.com/sn6000hw/1.3/specifications)。

边界：外壳/安装层级按公开外观组织；40柜与机房布局为展示。主镜头不验证每个隐藏接触。

### tray-midplane

PCB连接、背部中板与旧flyover概念差异

要讲清楚：PCB载板和结构frame；rear connectors到rack copper-cartridge关系；示意旧cable与新assembly区别。

素材ID：`tray-compute`, `board-compute`, `rack-nvl72`, `scene-pod-to-die`。

镜头：[02-rack-nvl72](SHOTS.md#02-rack-nvl72), [07-tray-compute](SHOTS.md#07-tray-compute), [24-pod-to-die](SHOTS.md#24-pod-to-die)。

原章节：nvl72:02。

近景：[assembled-detail](previews/tray-compute/assembled-detail.jpg) · [service-detail](previews/tray-compute/service-detail.jpg) · [pcb-detail](previews/tray-compute/pcb-detail.jpg)。

依据：[DGX Vera Rubin NVL72 hardware guide](https://docs.nvidia.com/dgx/dgxvr-user-guide/hardware.html) · [MGX 1.2 rack and trays design specification](https://www.opencompute.org/wp-content/uploads/2026/10/MGX-Accelerated-Computing-Rack-and-Trays-Specification-1.2.0-Final.pdf)。

边界：实体背部/中板用rear-detail；旧flyover只作版本解释，不声称两版真实硬件全共存。

### rubin-chiplet

Rubin双compute die、NVHBI与封装互联

要讲清楚：两die边界；die间短链路；HBM与interposer层。

素材ID：`chip-rubin`, `board-compute`, `tray-compute`。

镜头：[16-chip-rubin](SHOTS.md#16-chip-rubin), [07-tray-compute](SHOTS.md#07-tray-compute)。

原章节：nvl72:03.1, nvl72:08.2。

近景：[architecture-map](previews/chip-rubin/architecture-map.jpg) · [bare-die-schematic](previews/chip-rubin/bare-die-schematic.jpg) · [assembled-detail](previews/chip-rubin/assembled-detail.jpg)。

依据：[Inside the NVIDIA Vera Rubin platform: six new chips](https://developer.nvidia.com/blog/inside-the-nvidia-rubin-platform-six-new-chips-one-ai-supercomputer/) · [Inside NVIDIA Rubin GPU architecture](https://developer.nvidia.com/blog/inside-nvidia-rubin-gpu-architecture-powering-the-era-of-agentic-ai/)。

边界：双die/HBM/package是公开结构的owned geometry；内部区域不是显微物理floorplan。

### tensor-mac

矩阵MAC、operand复用、部分和累加

要讲清楚：operand A/B进入；MAC与accumulator；复用路径与输出。

素材ID：`gpu-tensor-dataflow`, `chip-rubin`, `chip-groq`。

镜头：[34-gpu-tensor-dataflow](SHOTS.md#34-gpu-tensor-dataflow), [16-chip-rubin](SHOTS.md#16-chip-rubin), [20-chip-groq](SHOTS.md#20-chip-groq)。

原章节：nvl72:03.3, lpx:04.2, lpx:11.2。

近景：[main-structure-detail](previews/gpu-tensor-dataflow/main-structure-detail.jpg) · [top](previews/gpu-tensor-dataflow/top.jpg) · [hero](previews/gpu-tensor-dataflow/hero.jpg)。

依据：[Inside NVIDIA Rubin GPU architecture](https://developer.nvidia.com/blog/inside-nvidia-rubin-gpu-architecture-powering-the-era-of-agentic-ai/) · [Groq3LPX compiler scheduled networking and long-context inference](https://developer.nvidia.com/blog/how-nvidia-groq-3-lpx-unlocks-ultrafast-interactivity-at-long-context-on-nvidia-vera-rubin/)。

边界：公开能力用owned放大示意说明；不声称供应商physical floorplan、逐周期RTL、真实工艺比例或测量。

### nvfp4-format

NVFP4位布局与分层scale

要讲清楚：1sign/2exponent/1mantissa；16值block E4M3 scale；FP32 global scale与重建。

素材ID：`nvfp4-block-scaling`, `gpu-tensor-dataflow`。

镜头：[53-nvfp4-block-scaling](SHOTS.md#53-nvfp4-block-scaling)。

原章节：nvl72:03.2-03.3。

近景：[main-structure-detail](previews/nvfp4-block-scaling/main-structure-detail.jpg) · [top](previews/nvfp4-block-scaling/top.jpg) · [hero](previews/nvfp4-block-scaling/hero.jpg)。

依据：[NVFP4 hierarchical block scaling in Transformer Engine2.20.2](https://docs.nvidia.com/deeplearning/transformer-engine/features/low_precision_training/nvfp4/nvfp4.html)。

边界：公开能力用owned放大示意说明；不声称供应商physical floorplan、逐周期RTL、真实工艺比例或测量。

### hbm-dram-stack

HBM4 DRAM堆叠与base logic

要讲清楚：各DRAM层与独立base；沿stack的数据/供电；assembly平盖与放大cutaway区别。

素材ID：`hbm4`, `hbm4-tsv`。

镜头：[22-hbm4-section](SHOTS.md#22-hbm4-section), [28-hbm4-tsv](SHOTS.md#28-hbm4-tsv)。

原章节：nvl72:03.4, lpx:05.1。

近景：[assembled-detail](previews/hbm4/assembled-detail.jpg) · [service-detail](previews/hbm4/service-detail.jpg) · [pcb-detail](previews/hbm4/pcb-detail.jpg)。

依据：[Micron HBM4](https://www.micron.com/products/memory/hbm/hbm4) · [SK hynix and TSMC HBM4 collaboration](https://news.skhynix.com/en/sk-hynix-partners-with-tsmc-to-strengthen-hbm-technological-leadership/)。

边界：公开能力用owned放大示意说明；不声称供应商physical floorplan、逐周期RTL、真实工艺比例或测量。

### hbm-tsv-bumps

TSV全硅厚度、微凸点与跨层导通

要讲清楚：穿透整层Si的TSV；相邻die之间bump；连续导电路径及分离的dielectric。

素材ID：`hbm4-tsv`。

镜头：[28-hbm4-tsv](SHOTS.md#28-hbm4-tsv)。

原章节：nvl72:03.4, lpx:05.1。

近景：[main-structure-detail](previews/hbm4-tsv/main-structure-detail.jpg) · [top](previews/hbm4-tsv/top.jpg) · [hero](previews/hbm4-tsv/hero.jpg)。

依据：[Creating new values in DRAM using Through Silicon Via technology](https://news.skhynix.com/en/creating-new-values-in-dram-using-through-silicon-via-technology-for-continued-scaling-in-memory-system-performance-and-capacity/) · [Advanced Memory Package Architecture](https://research-user.skhynix.com/research-areas/advanced-package/advanced-memory-package-architecture)。

边界：贯硅Cu、liner与层间bump的泛用截面；实际pitch/膜厚/接合工艺未复刻。

### hbm-interposer

2.5D interposer、redistribution与GPU/HBM连接

要讲清楚：GPU与HBM同interposer；vertical bump与horizontal routes；package substrate层。

素材ID：`chip-rubin`, `hbm4-tsv`。

镜头：[16-chip-rubin](SHOTS.md#16-chip-rubin), [28-hbm4-tsv](SHOTS.md#28-hbm4-tsv)。

原章节：nvl72:03.1-03.4。

近景：[architecture-map](previews/chip-rubin/architecture-map.jpg) · [bare-die-schematic](previews/chip-rubin/bare-die-schematic.jpg) · [assembled-detail](previews/chip-rubin/assembled-detail.jpg)。

依据：[SK hynix and TSMC HBM4 collaboration](https://news.skhynix.com/en/sk-hynix-partners-with-tsmc-to-strengthen-hbm-technological-leadership/) · [Inside NVIDIA Rubin GPU architecture](https://developer.nvidia.com/blog/inside-nvidia-rubin-gpu-architecture-powering-the-era-of-agentic-ai/)。

边界：2.5D横向fanout为代表走线，不是完整RDL mask。

### hbm-parallel-interface

宽并行HBM通路与外部串行PHY的区别

要讲清楚：多parallel data conductors；clock/control与data区别；对照serial channel，不将TSV当SerDes。

素材ID：`hbm4-tsv`, `memory-hierarchy`, `serdes-pam4`。

镜头：[28-hbm4-tsv](SHOTS.md#28-hbm4-tsv), [45-serdes-pam4](SHOTS.md#45-serdes-pam4)。

原章节：nvl72:03.4。

近景：[functional-parallel-hbm-link](previews/hbm4-tsv/functional-parallel-hbm-link.jpg) · [main-structure-detail](previews/hbm4-tsv/main-structure-detail.jpg) · [top](previews/hbm4-tsv/top.jpg)。

依据：[Micron HBM4](https://www.micron.com/products/memory/hbm/hbm4) · [DS560DF810 56Gbps multirate retimer datasheet RevB](https://www.ti.com/lit/ds/symlink/ds560df810.pdf)。

边界：六DATA+CMD+CLOCK仅8代表路线，不计作真实pin数或精确时序。

### dram1t1c

DRAM1T1C charge sharing与refresh

要讲清楚：1access MOS+1capacitor；plate/wordline/bitline；leakage→sense→restore/refresh。

素材ID：`memory-cell-dram1t1c`, `memory-cell-comparison`。

镜头：[26-memory-cell-dram1t1c](SHOTS.md#26-memory-cell-dram1t1c), [27-memory-cell-comparison](SHOTS.md#27-memory-cell-comparison)。

原章节：nvl72:03.4, lpx:05.1, stx:05.1。

近景：[main-structure-detail](previews/memory-cell-dram1t1c/main-structure-detail.jpg) · [functional-array-periphery](previews/memory-cell-dram1t1c/functional-array-periphery.jpg) · [top](previews/memory-cell-dram1t1c/top.jpg)。

依据：[MIT6.004: memory cells, cache lookup and generic coherence principles](https://ocw.mit.edu/courses/6-004-computation-structures-spring-2017/pages/c14/c14s1/)。

边界：1T1C、charge sharing/restore/leakage/refresh为normalized示意，不是器件瞬态求解。

### numa-c2c-coherence

C2C共享地址与本地/远端NUMA代价

要讲清楚：local versus remote access；coherent request/data；只有公开domain内共享，不把256CPU当一全域。

素材ID：`cpu-scf-coherence`, `board-vera`, `board-compute`, `tray-vera`, `tray-compute`。

镜头：[36-cpu-scf-coherence](SHOTS.md#36-cpu-scf-coherence), [09-tray-vera](SHOTS.md#09-tray-vera), [07-tray-compute](SHOTS.md#07-tray-compute)。

原章节：nvl72:04.3, vera:02.1-02.2, vera:04.4。

近景：[main-structure-detail](previews/cpu-scf-coherence/main-structure-detail.jpg) · [top](previews/cpu-scf-coherence/top.jpg) · [hero](previews/cpu-scf-coherence/hero.jpg)。

依据：[Inside the NVIDIA Vera Rubin platform: six new chips](https://developer.nvidia.com/blog/inside-the-nvidia-rubin-platform-six-new-chips-one-ai-supercomputer/) · [NVIDIA Vera CPU Architecture Whitepaper v1.12](https://nvdam.nvidia.com/Share/qkf77fo0u75m4o03ifxkae0a151h2b6k)。

边界：公开能力用owned放大示意说明；不声称供应商physical floorplan、逐周期RTL、真实工艺比例或测量。

### spatial-multithreading

双thread上下文与空间资源分区

要讲清楚：两上下文；partitioned frontend/queues/resources；88cores/176threads是架构数，不仿物理mask。

素材ID：`cpu-olympus-pipeline`, `chip-vera`。

镜头：[35-cpu-olympus-pipeline](SHOTS.md#35-cpu-olympus-pipeline), [15-chip-vera](SHOTS.md#15-chip-vera)。

原章节：nvl72:04.2, vera:03.7。

近景：[main-structure-detail](previews/cpu-olympus-pipeline/main-structure-detail.jpg) · [top](previews/cpu-olympus-pipeline/top.jpg) · [hero](previews/cpu-olympus-pipeline/hero.jpg)。

依据：[NVIDIA Vera CPU Architecture Whitepaper v1.12](https://nvdam.nvidia.com/Share/qkf77fo0u75m4o03ifxkae0a151h2b6k)。

边界：公开能力用owned放大示意说明；不声称供应商physical floorplan、逐周期RTL、真实工艺比例或测量。

### socamm-compression

SOCAMM2近CPU布置与压接

要讲清楚：三retention位置；back compression-pad阵列与socket；CPU旁8module bank与冷板遮挡关系。

素材ID：`socamm2`, `board-compute`, `board-vera`, `tray-compute`, `tray-vera`。

镜头：[07-tray-compute](SHOTS.md#07-tray-compute), [09-tray-vera](SHOTS.md#09-tray-vera)。

原章节：nvl72:02, vera:04.3。

近景：[assembled-detail](previews/socamm2/assembled-detail.jpg) · [service-detail](previews/socamm2/service-detail.jpg) · [pcb-detail](previews/socamm2/pcb-detail.jpg)。

依据：[Micron SOCAMM2 product and256GB release](https://www.micron.com/products/memory/lpddr-modules/socamm) · [SK hynix 192GB SOCAMM2 mass production and official product photograph](https://news.skhynix.com/en/mass-production-socamm2-192gb-2/) · [NVIDIA Vera CPU Architecture Whitepaper v1.12](https://nvdam.nvidia.com/Share/qkf77fo0u75m4o03ifxkae0a151h2b6k)。

边界：SOCAMM2及压接背面已有独立静态近景；没有独立57组SOCAMM动画，借07/09上下文。

### mesh-vs-switched

all-to-all通信、物理mesh与switched fabric

要讲清楚：N²直连对照switch接入；每endpoint路由；all-to-all能力不等同物理fullmesh。

素材ID：`network-mesh-fabric`。

镜头：[40-network-mesh-fabric](SHOTS.md#40-network-mesh-fabric)。

原章节：nvl72:05.1, nvl72:08.3。

近景：[main-structure-detail](previews/network-mesh-fabric/main-structure-detail.jpg) · [top](previews/network-mesh-fabric/top.jpg) · [hero](previews/network-mesh-fabric/hero.jpg)。

依据：[Inside the NVIDIA Vera Rubin platform: six new chips](https://developer.nvidia.com/blog/inside-the-nvidia-rubin-platform-six-new-chips-one-ai-supercomputer/)。

边界：公开能力用owned放大示意说明；不声称供应商physical floorplan、逐周期RTL、真实工艺比例或测量。

### passive-copper-spine

NVLink copper spine与rack rear cartridges

要讲清楚：四cartridge边界；tray电连接mating；signal铜缆与水铜管分开。

素材ID：`rack-nvl72`, `tray-nvlink`, `tray-compute`, `rack-vera`。

镜头：[02-rack-nvl72](SHOTS.md#02-rack-nvl72), [07-tray-compute](SHOTS.md#07-tray-compute), [08-tray-nvlink](SHOTS.md#08-tray-nvlink), [03-rack-vera](SHOTS.md#03-rack-vera)。

原章节：nvl72:05.2-05.5, vera:05.1。

近景：[assembled-detail](previews/rack-nvl72/assembled-detail.jpg) · [service-detail](previews/rack-nvl72/service-detail.jpg) · [pcb-detail](previews/rack-nvl72/pcb-detail.jpg)。

依据：[NVIDIA Vera Rubin POD: seven chips and five rack-scale systems](https://developer.nvidia.com/blog/nvidia-vera-rubin-pod-seven-chips-five-rack-scale-systems-one-ai-supercomputer/) · [DGX Vera Rubin NVL72 hardware guide](https://docs.nvidia.com/dgx/dgxvr-user-guide/hardware.html)。

边界：实体rear-connector近景补充机柜外观镜头；不推断未知针脚协议和导体公差。

### sharp-reduction

网络内reduce与broadcast

要讲清楚：多端点部分和；switch归约；结果广播；不称光路浮点计算。

素材ID：`network-sharp-reduction`, `chip-nvlink`。

镜头：[41-network-sharp-reduction](SHOTS.md#41-network-sharp-reduction), [17-chip-nvlink](SHOTS.md#17-chip-nvlink)。

原章节：nvl72:05.4, nvl72:08.3。

近景：[main-structure-detail](previews/network-sharp-reduction/main-structure-detail.jpg) · [top](previews/network-sharp-reduction/top.jpg) · [hero](previews/network-sharp-reduction/hero.jpg)。

依据：[Inside the NVIDIA Vera Rubin platform: six new chips](https://developer.nvidia.com/blog/inside-the-nvidia-rubin-platform-six-new-chips-one-ai-supercomputer/)。

边界：公开能力用owned放大示意说明；不声称供应商physical floorplan、逐周期RTL、真实工艺比例或测量。

### rdma-gpudirect

NIC直接DMA GPU memory路径

要讲清楚：NIC→PCIe→GPU memory；host staging对照；CPU setup/control仍存在。

素材ID：`rdma-astra-data-path`, `chip-cx9`。

镜头：[42-rdma-astra-data-path](SHOTS.md#42-rdma-astra-data-path), [18-chip-cx9](SHOTS.md#18-chip-cx9)。

原章节：nvl72:06.2, stx:03.2, stx:06。

近景：[main-structure-detail](previews/rdma-astra-data-path/main-structure-detail.jpg) · [top](previews/rdma-astra-data-path/top.jpg) · [hero](previews/rdma-astra-data-path/hero.jpg)。

依据：[GPUDirect RDMA13.4 documentation](https://docs.nvidia.com/cuda/gpudirect-rdma/index.html) · [Scaling agentic AI factories with NVIDIA BlueField](https://developer.nvidia.com/blog/scaling-agentic-ai-factories-through-extreme-co-design-with-nvidia-bluefield/)。

边界：公开能力用owned放大示意说明；不声称供应商physical floorplan、逐周期RTL、真实工艺比例或测量。

### rdma-registration-protection

注册/固定内存与地址权限边界

要讲清楚：registration/pinning；地址窗口与access keys概念；data path安全边界。

素材ID：`rdma-astra-data-path`。

镜头：[42-rdma-astra-data-path](SHOTS.md#42-rdma-astra-data-path)。

原章节：nvl72:06.2。

近景：[functional-processor-mr-registration](previews/rdma-astra-data-path/functional-processor-mr-registration.jpg) · [functional-processor-allow-deny](previews/rdma-astra-data-path/functional-processor-allow-deny.jpg) · [functional-processor-rdma-delivery](previews/rdma-astra-data-path/functional-processor-rdma-delivery.jpg)。

依据：[GPUDirect RDMA13.4 documentation](https://docs.nvidia.com/cuda/gpudirect-rdma/index.html) · [RDMA Aware Networks Programming User Manual1.7: memory regions and permissions](https://docs.nvidia.com/rdma-aware-networks-programming-user-manual-1-7.pdf)。

边界：公开能力用owned放大示意说明；不声称供应商physical floorplan、逐周期RTL、真实工艺比例或测量。

### astra-control-data-domains

Astra/DPU独立控制与数据域

要讲清楚：independent management control；tenant data path；GraceDPU与VeraSTX分版本。

素材ID：`rdma-astra-data-path`, `chip-bf4-dpu`, `chip-bf4-stx`。

镜头：[42-rdma-astra-data-path](SHOTS.md#42-rdma-astra-data-path), [19-chip-bf4-dpu](SHOTS.md#19-chip-bf4-dpu)。

原章节：nvl72:06.4, vera:06, stx:04.1-04.2。

近景：[functional-processor-bf4-control](previews/rdma-astra-data-path/functional-processor-bf4-control.jpg) · [main-structure-detail](previews/rdma-astra-data-path/main-structure-detail.jpg) · [top](previews/rdma-astra-data-path/top.jpg)。

依据：[Scaling agentic AI factories with NVIDIA BlueField](https://developer.nvidia.com/blog/scaling-agentic-ai-factories-through-extreme-co-design-with-nvidia-bluefield/)。

边界：公开能力用owned放大示意说明；不声称供应商physical floorplan、逐周期RTL、真实工艺比例或测量。

### packet-pipeline

Ethernet ingress→parse/lookup→buffer→egress

要讲清楚：header parse与forwarding决定；shared buffer与queue；scheduler/crossbar角色，非S6实际宏floorplan。

素材ID：`switch-packet-pipeline`, `chip-spectrum`。

镜头：[43-switch-packet-pipeline](SHOTS.md#43-switch-packet-pipeline), [21-chip-spectrum](SHOTS.md#21-chip-spectrum)。

原章节：nvl72:05.3, spx:02.1-02.3。

近景：[main-structure-detail](previews/switch-packet-pipeline/main-structure-detail.jpg) · [top](previews/switch-packet-pipeline/top.jpg) · [hero](previews/switch-packet-pipeline/hero.jpg)。

依据：[NVIDIA Spectrum-6 SN6000 Switch Systems Hardware User Manual 1.3](https://networking-docs.nvidia.com/sn6000hw/1.3/specifications) · [Fully shared packet buffering in NVIDIA Spectrum Ethernet](https://developer.nvidia.com/blog/maximizing-network-performance-for-storage-with-nvidia-spectrum-ethernet/)。

边界：解析/查询/shared buffer/egress的typical功能，不声明Spectrum物理floorplan、bank数。

### queue-hol-incast

incast、queue build-up与HOL

要讲清楚：多发送端涌入同出口；队列积累；pause/节流/回压范围区别。

素材ID：`network-incast-control`, `switch-packet-pipeline`。

镜头：[44-network-incast-control](SHOTS.md#44-network-incast-control), [43-switch-packet-pipeline](SHOTS.md#43-switch-packet-pipeline)。

原章节：nvl72:05.3, nvl72:06.3, spx:08.1。

近景：[main-structure-detail](previews/network-incast-control/main-structure-detail.jpg) · [top](previews/network-incast-control/top.jpg) · [hero](previews/network-incast-control/hero.jpg)。

依据：[Giga-scale Spectrum-X Ethernet and multiplane networking](https://developer.nvidia.com/blog/giga-scale-ai-ethernet-evolution-spectrum-x-ethernet-rewrites-rules/) · [Fully shared packet buffering in NVIDIA Spectrum Ethernet](https://developer.nvidia.com/blog/maximizing-network-performance-for-storage-with-nvidia-spectrum-ethernet/)。

边界：owned示意队列/反馈；不发明ECN阈值或从动画推断稳定性。

### ar-tcc-plb

AR/TCC/PLB不同位置的拥塞控制

要讲清楚：switch AR择路；endpoint TCC发送节流；NIC PLB选择plane。

素材ID：`network-incast-control`, `network-multiplane`。

镜头：[44-network-incast-control](SHOTS.md#44-network-incast-control), [50-network-multiplane](SHOTS.md#50-network-multiplane)。

原章节：nvl72:06.3, vera:05.4, spx:08.1-08.2。

近景：[main-structure-detail](previews/network-incast-control/main-structure-detail.jpg) · [top](previews/network-incast-control/top.jpg) · [hero](previews/network-incast-control/hero.jpg)。

依据：[Giga-scale Spectrum-X Ethernet and multiplane networking](https://developer.nvidia.com/blog/giga-scale-ai-ethernet-evolution-spectrum-x-ethernet-rewrites-rules/)。

边界：控制所在位置及分工的概念视图，不是策略RTL或性能实验。

### osfp-vs-cpo

可插OSFP和CPO的电/光边界

要讲清楚：长PCB电通道到pluggable；短package通道到PIC；ELS独立，电信号做逻辑，光传数据。

素材ID：`cpo-engine`, `chip-spectrum`, `tray-etl`, `switch-sn6810`。

镜头：[12-tray-etl](SHOTS.md#12-tray-etl), [14-switch-sn6810](SHOTS.md#14-switch-sn6810), [21-chip-spectrum](SHOTS.md#21-chip-spectrum), [23-cpo-engine](SHOTS.md#23-cpo-engine)。

原章节：nvl72:09, spx:04.1-04.3。

近景：[assembled-detail](previews/cpo-engine/assembled-detail.jpg) · [service-detail](previews/cpo-engine/service-detail.jpg) · [pcb-detail](previews/cpo-engine/pcb-detail.jpg)。

依据：[How industry collaboration fosters NVIDIA co-packaged optics](https://developer.nvidia.com/blog/how-industry-collaboration-fosters-nvidia-co-packaged-optics/) · [Scaling AI factories with co-packaged optics](https://developer.nvidia.com/blog/scaling-ai-factories-with-co-packaged-optics-for-better-power-efficiency/)。

边界：公开能力用owned放大示意说明；不声称供应商physical floorplan、逐周期RTL、真实工艺比例或测量。

### liquid-heat-path

die→TIM→coldplate→coolant→CDU热流

要讲清楚：TIM接触界面；microchannel流向；supply/return到CDU；45°C进水不等于junction。

素材ID：`liquid-cooling-section`, `tray-compute`, `room`。

镜头：[55-liquid-cooling-section](SHOTS.md#55-liquid-cooling-section), [07-tray-compute](SHOTS.md#07-tray-compute), [01-pod-tour](SHOTS.md#01-pod-tour)。

原章节：nvl72:07.1-07.2, vera:07.1, lpx:09.4。

近景：[functional-coldplate-section](previews/liquid-cooling-section/functional-coldplate-section.jpg) · [main-structure-detail](previews/liquid-cooling-section/main-structure-detail.jpg) · [assembled-detail](previews/liquid-cooling-section/assembled-detail.jpg)。

依据：[DGX Vera Rubin NVL72 hardware guide](https://docs.nvidia.com/dgx/dgxvr-user-guide/hardware.html) · [MGX 1.2 rack and trays design specification](https://www.opencompute.org/wp-content/uploads/2026/10/MGX-Accelerated-Computing-Rack-and-Trays-Specification-1.2.0-Final.pdf)。

边界：generic冷板截面与供回液，不是实测流量/压降/热接触。

### liquid-qd-service

blind-mate QD/valve与tray维护

要讲清楚：inlet/outlet实体空口；断开时阀闭合示意；water与signal connector严格分开。

素材ID：`liquid-cooling-section`, `tray-compute`, `tray-nvlink`。

镜头：[55-liquid-cooling-section](SHOTS.md#55-liquid-cooling-section), [07-tray-compute](SHOTS.md#07-tray-compute), [08-tray-nvlink](SHOTS.md#08-tray-nvlink)。

原章节：nvl72:07.2, vera:07.1。

近景：[functional-uqd-section](previews/liquid-cooling-section/functional-uqd-section.jpg) · [main-structure-detail](previews/liquid-cooling-section/main-structure-detail.jpg) · [assembled-detail](previews/liquid-cooling-section/assembled-detail.jpg)。

依据：[MGX 1.2 rack and trays design specification](https://www.opencompute.org/wp-content/uploads/2026/10/MGX-Accelerated-Computing-Rack-and-Trays-Specification-1.2.0-Final.pdf) · [DGX Vera Rubin NVL72 hardware guide](https://docs.nvidia.com/dgx/dgxvr-user-guide/hardware.html)。

边界：弹簧poppet开合教学，不是具体厂商阀座/密封或工程接触验证。

### busbar-power-path

54V电源架→busbar→PDB与IR损耗

要讲清楚：power shelf与rear bar；branch进入trayPDB；高电流导体/液冷与I²R示意。

素材ID：`power-vrm-pdn`, `rack-nvl72`, `tray-compute`。

镜头：[56-power-vrm-pdn](SHOTS.md#56-power-vrm-pdn), [02-rack-nvl72](SHOTS.md#02-rack-nvl72), [07-tray-compute](SHOTS.md#07-tray-compute)。

原章节：nvl72:07.3。

近景：[main-structure-detail](previews/power-vrm-pdn/main-structure-detail.jpg) · [assembled-detail](previews/power-vrm-pdn/assembled-detail.jpg) · [service-detail](previews/power-vrm-pdn/service-detail.jpg)。

依据：[DGX Vera Rubin NVL72 hardware guide](https://docs.nvidia.com/dgx/dgxvr-user-guide/hardware.html) · [TI SLVA882B: Multiphase Buck Design From Start to Finish](https://www.ti.com/lit/an/slva882b/slva882b.pdf)。

边界：公开能力用owned放大示意说明；不声称供应商physical floorplan、逐周期RTL、真实工艺比例或测量。

### rack-power-smoothing

rack储能、power floor与smoothing

要讲清楚：负载脉冲与电网输入；energy buffer charge/discharge；power floor和容量约束分别说明。

素材ID：`power-smoothing`, `rack-nvl72`。

镜头：[57-power-smoothing](SHOTS.md#57-power-smoothing), [02-rack-nvl72](SHOTS.md#02-rack-nvl72)。

原章节：nvl72:07.4。

近景：[main-structure-detail](previews/power-smoothing/main-structure-detail.jpg) · [assembled-detail](previews/power-smoothing/assembled-detail.jpg) · [service-detail](previews/power-smoothing/service-detail.jpg)。

依据：[Inside the NVIDIA Vera Rubin platform: six new chips](https://developer.nvidia.com/blog/inside-the-nvidia-rubin-platform-six-new-chips-one-ai-supercomputer/) · [Groq3LPX deterministic execution and proactive power control](https://developer.nvidia.com/blog/how-nvidia-groq-3-lpx-deterministic-execution-drives-power-efficient-high-interactivity-inference-on-nvidia-vera-rubin/)。

边界：公开能力用owned放大示意说明；不声称供应商physical floorplan、逐周期RTL、真实工艺比例或测量。

### ras-repair-maintenance

ECC/RAS、冗余路径与维护范围

要讲清楚：memory错误→纠错/报告；坏link→reroute；switch维修和compute离线的影响不同。

素材ID：`network-multiplane`, `memory-hierarchy`, `rack-nvl72`, `lpu-c2c-network`。

镜头：[38-lpu-c2c-network](SHOTS.md#38-lpu-c2c-network), [50-network-multiplane](SHOTS.md#50-network-multiplane)。

原章节：nvl72:07.5, vera:07.3。

近景：[functional-timing-detail-fault-reroute-maintenance](previews/network-multiplane/functional-timing-detail-fault-reroute-maintenance.jpg) · [main-structure-detail](previews/network-multiplane/main-structure-detail.jpg) · [top](previews/network-multiplane/top.jpg)。

依据：[Inside the NVIDIA Vera Rubin platform: six new chips](https://developer.nvidia.com/blog/inside-the-nvidia-rubin-platform-six-new-chips-one-ai-supercomputer/) · [NVIDIA Vera CPU Architecture Whitepaper v1.12](https://nvdam.nvidia.com/Share/qkf77fo0u75m4o03ifxkae0a151h2b6k)。

边界：教材SECDED单错更正/双错检测与健康路径reroute分开；reroute不是bit correction。

### package-comparison-principles

monolithic/chiplet/2.5D/3D异构封装原理

要讲清楚：单die与multi-die边界；横向interposer与垂直bond；跨die接口开销。

素材ID：`chip-rubin`, `chip-vera`, `hbm4-tsv`, `cpo-package-section`。

镜头：[49-cpo-package-section](SHOTS.md#49-cpo-package-section), [16-chip-rubin](SHOTS.md#16-chip-rubin), [15-chip-vera](SHOTS.md#15-chip-vera), [28-hbm4-tsv](SHOTS.md#28-hbm4-tsv)。

原章节：nvl72:08.2-08.4, vera:09, lpx:11.3。

近景：[architecture-map](previews/chip-rubin/architecture-map.jpg) · [bare-die-schematic](previews/chip-rubin/bare-die-schematic.jpg) · [assembled-detail](previews/chip-rubin/assembled-detail.jpg)。

依据：[Inside NVIDIA Rubin GPU architecture](https://developer.nvidia.com/blog/inside-nvidia-rubin-gpu-architecture-powering-the-era-of-agentic-ai/) · [NVIDIA Vera CPU Architecture Whitepaper v1.12](https://nvdam.nvidia.com/Share/qkf77fo0u75m4o03ifxkae0a151h2b6k) · [SK hynix and TSMC HBM4 collaboration](https://news.skhynix.com/en/sk-hynix-partners-with-tsmc-to-strengthen-hbm-technological-leadership/)。

边界：公开能力用owned放大示意说明；不声称供应商physical floorplan、逐周期RTL、真实工艺比例或测量。

## Vera CPU Rack

### memory-hierarchy

register/cache/SRAM/DRAM/HBM/SSD容量与局部性

要讲清楚：计算单元旁cache与内存角色；命中/缺失路径；容量/latency示意，不伪造固定几层。

素材ID：`memory-hierarchy`, `kv-cache-tiers`。

镜头：[29-memory-hierarchy](SHOTS.md#29-memory-hierarchy), [33-kv-cache-tiers](SHOTS.md#33-kv-cache-tiers)。

原章节：vera:04, lpx:04.5-05.4, stx:06.1。

近景：[main-structure-detail](previews/memory-hierarchy/main-structure-detail.jpg) · [top](previews/memory-hierarchy/top.jpg) · [hero](previews/memory-hierarchy/hero.jpg)。

依据：[MIT6.004: memory cells, cache lookup and generic coherence principles](https://ocw.mit.edu/courses/6-004-computation-structures-spring-2017/pages/c14/c14s1/) · [Introducing BlueField-4-powered CMX context memory storage](https://developer.nvidia.com/blog/introducing-nvidia-bluefield-4-powered-inference-context-memory-storage-platform-for-the-next-frontier-of-ai/)。

边界：公开能力用owned放大示意说明；不声称供应商physical floorplan、逐周期RTL、真实工艺比例或测量。

### cache-array-banks

cache tag/data、bank、仲裁与局部性

要讲清楚：地址→tag/data；hit/miss分支；bank并行与冲突。

素材ID：`memory-hierarchy`, `cpu-scf-coherence`, `chip-vera`, `lpu-static-schedule`。

镜头：[29-memory-hierarchy](SHOTS.md#29-memory-hierarchy), [37-lpu-static-schedule](SHOTS.md#37-lpu-static-schedule), [36-cpu-scf-coherence](SHOTS.md#36-cpu-scf-coherence)。

原章节：vera:03.5, vera:04.1, lpx:05.2-05.3。

近景：[functional-cache-lookup](previews/memory-hierarchy/functional-cache-lookup.jpg) · [main-structure-detail](previews/memory-hierarchy/main-structure-detail.jpg) · [top](previews/memory-hierarchy/top.jpg)。

依据：[MIT6.004: memory cells, cache lookup and generic coherence principles](https://ocw.mit.edu/courses/6-004-computation-structures-spring-2017/pages/c14/c14s1/) · [NVIDIA Vera CPU Architecture Whitepaper v1.12](https://nvdam.nvidia.com/Share/qkf77fo0u75m4o03ifxkae0a151h2b6k)。

边界：cache tag/data、仲裁与cell技术分层，不把所有cache块叫单个6T cell。

### vera-io-phy-bifurcation

IO/PHY、PCIe端口分割与CXL

要讲清楚：8LPDDRCTRL与SystemIO逻辑区域；PCIe x16→x8/x4/x2分割；PHY功能接口带，非认证宏位置。

素材ID：`chip-vera`, `cxl-vs-cmx`, `serdes-pam4`, `cpu-olympus-pipeline`。

镜头：[35-cpu-olympus-pipeline](SHOTS.md#35-cpu-olympus-pipeline), [51-cxl-vs-cmx](SHOTS.md#51-cxl-vs-cmx), [15-chip-vera](SHOTS.md#15-chip-vera)。

原章节：vera:03.8, vera:05.3, stx:03.3。

近景：[architecture-map](previews/chip-vera/architecture-map.jpg) · [bare-die-schematic](previews/chip-vera/bare-die-schematic.jpg) · [assembled-detail](previews/chip-vera/assembled-detail.jpg)。

依据：[NVIDIA Vera CPU Architecture Whitepaper v1.12](https://nvdam.nvidia.com/Share/qkf77fo0u75m4o03ifxkae0a151h2b6k) · [CXL Consortium: coherent memory and host load/store semantics](https://computeexpresslink.org/blog/questions-from-the-compute-express-link-exploring-coherent-memory-and-innovative-use-cases-webinar-2341/)。

边界：同16lane的替代宽度分组；PHY收发功能与core/cache分开，未复刻Flex IO晶体管电路。

### olympus-front-end

宽取指/10路decode与吞吐限制

要讲清楚：fetch/decode/rename分层；10输入道；依赖/执行/退休限制。

素材ID：`cpu-olympus-pipeline`, `chip-vera`。

镜头：[35-cpu-olympus-pipeline](SHOTS.md#35-cpu-olympus-pipeline), [15-chip-vera](SHOTS.md#15-chip-vera)。

原章节：vera:03.1-03.3。

近景：[main-structure-detail](previews/cpu-olympus-pipeline/main-structure-detail.jpg) · [top](previews/cpu-olympus-pipeline/top.jpg) · [hero](previews/cpu-olympus-pipeline/hero.jpg)。

依据：[NVIDIA Vera CPU Architecture Whitepaper v1.12](https://nvdam.nvidia.com/Share/qkf77fo0u75m4o03ifxkae0a151h2b6k)。

边界：公开能力用owned放大示意说明；不声称供应商physical floorplan、逐周期RTL、真实工艺比例或测量。

### branch-predictor

neural branch predictor、推测与冲刷

要讲清楚：branch history与预测路径；错误路径/flush；返回fetch的纠正。

素材ID：`cpu-olympus-pipeline`, `chip-vera`。

镜头：[35-cpu-olympus-pipeline](SHOTS.md#35-cpu-olympus-pipeline)。

原章节：vera:03.4。

近景：[main-structure-detail](previews/cpu-olympus-pipeline/main-structure-detail.jpg) · [functional-processor-branch](previews/cpu-olympus-pipeline/functional-processor-branch.jpg) · [functional-processor-branch-recovery](previews/cpu-olympus-pipeline/functional-processor-branch-recovery.jpg)。

依据：[NVIDIA Vera CPU Architecture Whitepaper v1.12](https://nvdam.nvidia.com/Share/qkf77fo0u75m4o03ifxkae0a151h2b6k)。

边界：公开能力+toy误预测/冲刷/恢复，不模拟neural predictor内部网络或真实恢复延迟。

### ooo-rename-commit

register rename、ROB、依赖与顺序提交

要讲清楚：architectural/physical rename关系；ready/wait与OoO execute；ROB按程序序commit。

素材ID：`cpu-olympus-pipeline`, `chip-vera`。

镜头：[35-cpu-olympus-pipeline](SHOTS.md#35-cpu-olympus-pipeline)。

原章节：vera:03.5。

近景：[main-structure-detail](previews/cpu-olympus-pipeline/main-structure-detail.jpg) · [functional-processor-rename](previews/cpu-olympus-pipeline/functional-processor-rename.jpg) · [top](previews/cpu-olympus-pipeline/top.jpg)。

依据：[NVIDIA Vera CPU Architecture Whitepaper v1.12](https://nvdam.nvidia.com/Share/qkf77fo0u75m4o03ifxkae0a151h2b6k)。

边界：四指令rename/ROB/ready-wait示例；执行与提交顺序分开，不把示例说成证明消除全部假依赖。

### memory-rename-value-prediction

store-to-load依赖、memory renaming/value prediction

要讲清楚：producer value→consumer；预测值与验证；错误时recovery。

素材ID：`cpu-olympus-pipeline`。

镜头：[35-cpu-olympus-pipeline](SHOTS.md#35-cpu-olympus-pipeline)。

原章节：vera:03.5。

近景：[functional-processor-forward](previews/cpu-olympus-pipeline/functional-processor-forward.jpg) · [functional-processor-value-prediction](previews/cpu-olympus-pipeline/functional-processor-value-prediction.jpg) · [main-structure-detail](previews/cpu-olympus-pipeline/main-structure-detail.jpg)。

依据：[NVIDIA Vera CPU Architecture Whitepaper v1.12](https://nvdam.nvidia.com/Share/qkf77fo0u75m4o03ifxkae0a151h2b6k)。

边界：转发13与预测42/真实40恢复两个例子；不是Vera预测算法或测量。

### graph-prefetch

producer-consumer间接寻址预取

要讲清楚：B[i] producer返回index；A[B[i]] consumer address；学习关系后提前prefetch到cache。

素材ID：`cpu-graph-prefetch`, `cpu-olympus-pipeline`。

镜头：[52-cpu-graph-prefetch](SHOTS.md#52-cpu-graph-prefetch), [35-cpu-olympus-pipeline](SHOTS.md#35-cpu-olympus-pipeline)。

原章节：vera:03.6。

近景：[main-structure-detail](previews/cpu-graph-prefetch/main-structure-detail.jpg) · [top](previews/cpu-graph-prefetch/top.jpg) · [hero](previews/cpu-graph-prefetch/hero.jpg)。

依据：[NVIDIA Vera CPU Architecture Whitepaper v1.12](https://nvdam.nvidia.com/Share/qkf77fo0u75m4o03ifxkae0a151h2b6k)。

边界：公开能力用owned放大示意说明；不声称供应商physical floorplan、逐周期RTL、真实工艺比例或测量。

### scf-nodes-slcs

SCF中的CSN/MSN/BSN与分布式SLC

要讲清楚：CSN最多2core；MSN→memory/BSN→C2C；多SLC slice形成统一164MBL3。

素材ID：`cpu-scf-coherence`, `chip-vera`。

镜头：[36-cpu-scf-coherence](SHOTS.md#36-cpu-scf-coherence), [15-chip-vera](SHOTS.md#15-chip-vera)。

原章节：vera:04.1-04.2。

近景：[main-structure-detail](previews/cpu-scf-coherence/main-structure-detail.jpg) · [top](previews/cpu-scf-coherence/top.jpg) · [hero](previews/cpu-scf-coherence/hero.jpg)。

依据：[NVIDIA Vera CPU Architecture Whitepaper v1.12](https://nvdam.nvidia.com/Share/qkf77fo0u75m4o03ifxkae0a151h2b6k)。

边界：Vera SLC=System-Level Cache；公开逻辑节点，不是实际硅布局。

### coherence-state

目录ownership、invalidation与cache coherence

要讲清楚：request→ownership→invalidate；dirty/shared state和data返回；memory ordering概念。

素材ID：`cpu-scf-coherence`。

镜头：[36-cpu-scf-coherence](SHOTS.md#36-cpu-scf-coherence)。

原章节：vera:02.1, vera:04.1。

近景：[functional-ownership-example](previews/cpu-scf-coherence/functional-ownership-example.jpg) · [main-structure-detail](previews/cpu-scf-coherence/main-structure-detail.jpg) · [top](previews/cpu-scf-coherence/top.jpg)。

依据：[NVIDIA Vera CPU Architecture Whitepaper v1.12](https://nvdam.nvidia.com/Share/qkf77fo0u75m4o03ifxkae0a151h2b6k) · [MIT6.004: memory cells, cache lookup and generic coherence principles](https://ocw.mit.edu/courses/6-004-computation-structures-spring-2017/pages/c14/c14s1/)。

边界：owned ownership/invalidation前后例子配路径，不是完整MESI或供应商协议RTL。

### agent-cpu-gpu-loop

GPU生成→CPU tool/sandbox→环境反馈

要讲清楚：CPU与GPU各自任务；返回token/工具结果；关键路径等待可见。

素材ID：`prefill-decode-split`, `cpu-olympus-pipeline`。

镜头：[39-prefill-decode-split](SHOTS.md#39-prefill-decode-split)。

原章节：vera:08。

近景：[main-structure-detail](previews/prefill-decode-split/main-structure-detail.jpg) · [top](previews/prefill-decode-split/top.jpg) · [hero](previews/prefill-decode-split/hero.jpg)。

依据：[NVIDIA Vera CPU: Olympus cores for agentic AI](https://developer.nvidia.com/blog/?p=120182) · [NVIDIA Vera CPU Architecture Whitepaper v1.12](https://nvdam.nvidia.com/Share/qkf77fo0u75m4o03ifxkae0a151h2b6k)。

边界：公开能力用owned放大示意说明；不声称供应商physical floorplan、逐周期RTL、真实工艺比例或测量。

### pcs-fec

SerDes后PCS/deskew/FEC/MAC层级

要讲清楚：physical sample→lane align→FEC→MAC；FEC修错与额外latency；具体码型未知。

素材ID：`serdes-equalization-cdr`, `switch-packet-pipeline`。

镜头：[46-serdes-equalization-cdr](SHOTS.md#46-serdes-equalization-cdr)。

原章节：vera:05.2-05.3, spx:03.1。

近景：[main-structure-detail](previews/serdes-equalization-cdr/main-structure-detail.jpg) · [functional-cdr-sampling](previews/serdes-equalization-cdr/functional-cdr-sampling.jpg) · [top](previews/serdes-equalization-cdr/top.jpg)。

依据：[NVIDIA Spectrum-6 SN6000 Switch Systems Hardware User Manual 1.3](https://networking-docs.nvidia.com/sn6000hw/1.3/specifications) · [DS560DF810 56Gbps multirate retimer datasheet RevB](https://www.ti.com/lit/ds/symlink/ds560df810.pdf)。

边界：公开能力用owned放大示意说明；不声称供应商physical floorplan、逐周期RTL、真实工艺比例或测量。

### pam4-nrz

NRZ/PAM4四电平、符号与眼图

要讲清楚：four symbol levels/two bits；differential wires；三眼与噪声margin，示意波形非实测。

素材ID：`serdes-pam4`。

镜头：[45-serdes-pam4](SHOTS.md#45-serdes-pam4)。

原章节：vera:05.3, spx:03.1。

近景：[main-structure-detail](previews/serdes-pam4/main-structure-detail.jpg) · [top](previews/serdes-pam4/top.jpg) · [hero](previews/serdes-pam4/hero.jpg)。

依据：[DS560DF810 56Gbps multirate retimer datasheet RevB](https://www.ti.com/lit/ds/symlink/ds560df810.pdf)。

边界：公开能力用owned放大示意说明；不声称供应商physical floorplan、逐周期RTL、真实工艺比例或测量。

### confidential-domains

CCA/RME、VM keys与独立安全域

要讲清楚：每VM保护域/keys；device assignment边界；控制域独立，不宣称绕过CPU安全。

素材ID：`rdma-astra-data-path`, `chip-vera`, `chip-bf4-dpu`, `cpu-olympus-pipeline`, `chip-bf4-stx`。

镜头：[35-cpu-olympus-pipeline](SHOTS.md#35-cpu-olympus-pipeline), [42-rdma-astra-data-path](SHOTS.md#42-rdma-astra-data-path), [19-chip-bf4-dpu](SHOTS.md#19-chip-bf4-dpu)。

原章节：vera:06, vera:07.3, stx:09。

近景：[functional-processor-bf4-control](previews/rdma-astra-data-path/functional-processor-bf4-control.jpg) · [main-structure-detail](previews/rdma-astra-data-path/main-structure-detail.jpg) · [top](previews/rdma-astra-data-path/top.jpg)。

依据：[NVIDIA Vera CPU Architecture Whitepaper v1.12](https://nvdam.nvidia.com/Share/qkf77fo0u75m4o03ifxkae0a151h2b6k) · [Scaling agentic AI factories with NVIDIA BlueField](https://developer.nvidia.com/blog/scaling-agentic-ai-factories-through-extreme-co-design-with-nvidia-bluefield/) · [Arm RME architecture: Realm isolation and four security states](https://neoverse-reference-design.docs.arm.com/en/latest/shared/rme.html)。

边界：PAS、Realm owner及授权TDISP-capable设备分条件；非物理RTL或实际安全攻击测试。

## Groq 3 LPX

### sram6t

SRAM6T交叉耦合与读写

要讲清楚：4latch MOS+2access MOS；Q/Qbar、WL、BL/BLbar；预充、sense与写入反馈。

素材ID：`memory-cell-sram6t`, `memory-cell-comparison`。

镜头：[25-memory-cell-sram6t](SHOTS.md#25-memory-cell-sram6t), [27-memory-cell-comparison](SHOTS.md#27-memory-cell-comparison)。

原章节：lpx:05.1, stx:05.1。

近景：[main-structure-detail](previews/memory-cell-sram6t/main-structure-detail.jpg) · [functional-array-periphery](previews/memory-cell-sram6t/functional-array-periphery.jpg) · [top](previews/memory-cell-sram6t/top.jpg)。

依据：[MIT6.004: memory cells, cache lookup and generic coherence principles](https://ocw.mit.edu/courses/6-004-computation-structures-spring-2017/pages/c14/c14s1/)。

边界：6T cross-coupled generic单元与WL/BL外围；保持在通电条件下，非真实工艺面积。

### cell-structure-comparison

SRAM/DRAM单元、外围电路与密度取舍

要讲清楚：同一教学放大尺度下结构对比；decoder/sense外围；明确不按nm或统一面积比例。

素材ID：`memory-cell-comparison`。

镜头：[27-memory-cell-comparison](SHOTS.md#27-memory-cell-comparison)。

原章节：lpx:05.1-05.5。

近景：[main-structure-detail](previews/memory-cell-comparison/main-structure-detail.jpg) · [functional-array-periphery](previews/memory-cell-comparison/functional-array-periphery.jpg) · [assembled-detail](previews/memory-cell-comparison/assembled-detail.jpg)。

依据：[MIT6.004: memory cells, cache lookup and generic coherence principles](https://ocw.mit.edu/courses/6-004-computation-structures-spring-2017/pages/c14/c14s1/)。

边界：比功能、外围与保持/刷新；放大模型尺寸不能作为工艺密度比。

### lpu-functional-engines

MEM/MXM/VXM/SXM功能与数据移动

要讲清楚：matrix/vector/transpose角色区别；compiler-managed SRAM；SXM reshape而非矩阵算子。

素材ID：`chip-groq`, `lpu-static-schedule`。

镜头：[20-chip-groq](SHOTS.md#20-chip-groq), [37-lpu-static-schedule](SHOTS.md#37-lpu-static-schedule)。

原章节：lpx:04.1-04.5。

近景：[architecture-map](previews/chip-groq/architecture-map.jpg) · [bare-die-schematic](previews/chip-groq/bare-die-schematic.jpg) · [assembled-detail](previews/chip-groq/assembled-detail.jpg)。

依据：[Inside NVIDIA Groq 3 LPX](https://developer.nvidia.com/blog/inside-nvidia-groq-3-lpx-the-low-latency-inference-accelerator-for-the-nvidia-vera-rubin-platform/) · [Groq3LPX deterministic execution and proactive power control](https://developer.nvidia.com/blog/how-nvidia-groq-3-lpx-deterministic-execution-drives-power-efficient-high-interactivity-inference-on-nvidia-vera-rubin/)。

边界：公开能力用owned放大示意说明；不声称供应商physical floorplan、逐周期RTL、真实工艺比例或测量。

### static-schedule

编译器排时、流式流水与compute/communication overlap

要讲清楚：compile前排时表；数据恰时到达；compute与transfer重叠，不是runtime自由乱序。

素材ID：`lpu-static-schedule`。

镜头：[37-lpu-static-schedule](SHOTS.md#37-lpu-static-schedule)。

原章节：lpx:06.1-06.3。

近景：[main-structure-detail](previews/lpu-static-schedule/main-structure-detail.jpg) · [functional-timing-detail-bank-conflict](previews/lpu-static-schedule/functional-timing-detail-bank-conflict.jpg) · [top](previews/lpu-static-schedule/top.jpg)。

依据：[Groq3LPX compiler scheduled networking and long-context inference](https://developer.nvidia.com/blog/how-nvidia-groq-3-lpx-unlocks-ultrafast-interactivity-at-long-context-on-nvidia-vera-rubin/) · [Groq3LPX deterministic execution and proactive power control](https://developer.nvidia.com/blog/how-nvidia-groq-3-lpx-deterministic-execution-drives-power-efficient-high-interactivity-inference-on-nvidia-vera-rubin/)。

边界：公开能力用owned放大示意说明；不声称供应商physical floorplan、逐周期RTL、真实工艺比例或测量。

### lpu-bank-conflicts

静态解决SRAM bank资源冲突

要讲清楚：两访问同bank冲突；分配不同slot；计划与执行对照。

素材ID：`lpu-static-schedule`, `memory-hierarchy`。

镜头：[37-lpu-static-schedule](SHOTS.md#37-lpu-static-schedule), [29-memory-hierarchy](SHOTS.md#29-memory-hierarchy)。

原章节：lpx:05.2, lpx:06.1-06.5。

近景：[functional-timing-detail-bank-conflict](previews/lpu-static-schedule/functional-timing-detail-bank-conflict.jpg) · [main-structure-detail](previews/lpu-static-schedule/main-structure-detail.jpg) · [top](previews/lpu-static-schedule/top.jpg)。

依据：[Groq3LPX deterministic execution and proactive power control](https://developer.nvidia.com/blog/how-nvidia-groq-3-lpx-deterministic-execution-drives-power-efficient-high-interactivity-inference-on-nvidia-vera-rubin/)。

边界：公开能力用owned放大示意说明；不声称供应商physical floorplan、逐周期RTL、真实工艺比例或测量。

### plesiosynchronous-clock

本地时钟协调与clock-domain时序

要讲清楚：多个clock domain；transfer时序协调；CPS周期变化与边界。

素材ID：`lpu-c2c-network`, `power-smoothing`, `lpu-static-schedule`。

镜头：[37-lpu-static-schedule](SHOTS.md#37-lpu-static-schedule)。

原章节：lpx:06.4。

近景：[main-structure-detail](previews/lpu-c2c-network/main-structure-detail.jpg) · [top](previews/lpu-c2c-network/top.jpg) · [hero](previews/lpu-c2c-network/hero.jpg)。

依据：[Groq3LPX deterministic execution and proactive power control](https://developer.nvidia.com/blog/how-nvidia-groq-3-lpx-deterministic-execution-drives-power-efficient-high-interactivity-inference-on-nvidia-vera-rubin/)。

边界：固定相位差、相近频率与协调窗口为通用教学；不是Groq clock实际漂移仿真。

### lpu-direct-c2c

direct C2C、跨tray路径与first-bit latency

要讲清楚：8端点/tray；direct route与可选multi-hop；aggregate/pairwise/bisection带宽区别。

素材ID：`lpu-c2c-network`, `rack-lpx`, `tray-lpx`。

镜头：[38-lpu-c2c-network](SHOTS.md#38-lpu-c2c-network), [04-rack-lpx](SHOTS.md#04-rack-lpx), [10-tray-lpx](SHOTS.md#10-tray-lpx)。

原章节：lpx:07.1-07.5。

近景：[main-structure-detail](previews/lpu-c2c-network/main-structure-detail.jpg) · [functional-timing-detail-distributed-capacity](previews/lpu-c2c-network/functional-timing-detail-distributed-capacity.jpg) · [top](previews/lpu-c2c-network/top.jpg)。

依据：[Inside NVIDIA Groq 3 LPX](https://developer.nvidia.com/blog/inside-nvidia-groq-3-lpx-the-low-latency-inference-accelerator-for-the-nvidia-vera-rubin-platform/) · [Groq3LPX compiler scheduled networking and long-context inference](https://developer.nvidia.com/blog/how-nvidia-groq-3-lpx-unlocks-ultrafast-interactivity-at-long-context-on-nvidia-vera-rubin/)。

边界：公开能力用owned放大示意说明；不声称供应商physical floorplan、逐周期RTL、真实工艺比例或测量。

### lpu-fel-dram

FEL/DRAM/host与LPU片上SRAM分工

要讲清楚：FEL连接扩展链路；external DRAM与on-chip MEM分开；hostCPU/BF4管理域；不称未证FPGA。

素材ID：`tray-lpx`, `board-lpx`, `lpu-c2c-network`, `lpu-static-schedule`。

镜头：[10-tray-lpx](SHOTS.md#10-tray-lpx), [38-lpu-c2c-network](SHOTS.md#38-lpu-c2c-network), [37-lpu-static-schedule](SHOTS.md#37-lpu-static-schedule)。

原章节：lpx:02.1-02.2。

近景：[assembled-detail](previews/tray-lpx/assembled-detail.jpg) · [service-detail](previews/tray-lpx/service-detail.jpg) · [pcb-detail](previews/tray-lpx/pcb-detail.jpg)。

依据：[Inside NVIDIA Groq 3 LPX](https://developer.nvidia.com/blog/inside-nvidia-groq-3-lpx-the-low-latency-inference-accelerator-for-the-nvidia-vera-rubin-platform/)。

边界：FEL/DRAM/host分角色；不称FEL为无证实的FPGA，也不推断隐藏carrier芯片人口。

### prefill-decode

Prefill矩阵与逐token Decode

要讲清楚：prompt并行矩阵；单token vector读weights/KV；stage间数据交接。

素材ID：`prefill-decode-split`。

镜头：[39-prefill-decode-split](SHOTS.md#39-prefill-decode-split)。

原章节：lpx:03.1-03.2, lpx:08。

近景：[main-structure-detail](previews/prefill-decode-split/main-structure-detail.jpg) · [top](previews/prefill-decode-split/top.jpg) · [hero](previews/prefill-decode-split/hero.jpg)。

依据：[Inside NVIDIA Groq 3 LPX](https://developer.nvidia.com/blog/inside-nvidia-groq-3-lpx-the-low-latency-inference-accelerator-for-the-nvidia-vera-rubin-platform/) · [Groq3LPX compiler scheduled networking and long-context inference](https://developer.nvidia.com/blog/how-nvidia-groq-3-lpx-unlocks-ultrafast-interactivity-at-long-context-on-nvidia-vera-rubin/)。

边界：公开能力用owned放大示意说明；不声称供应商physical floorplan、逐周期RTL、真实工艺比例或测量。

### attention-ffn

Attention/FFN拆分与KV读取

要讲清楚：Attention读K/V；FFN矩阵路径；每层跨系统的数据和协调成本。

素材ID：`prefill-decode-split`, `kv-cache-tiers`。

镜头：[39-prefill-decode-split](SHOTS.md#39-prefill-decode-split), [33-kv-cache-tiers](SHOTS.md#33-kv-cache-tiers)。

原章节：lpx:08, stx:01.1。

近景：[main-structure-detail](previews/prefill-decode-split/main-structure-detail.jpg) · [functional-kv-tensor](previews/prefill-decode-split/functional-kv-tensor.jpg) · [top](previews/prefill-decode-split/top.jpg)。

依据：[Inside NVIDIA Groq 3 LPX](https://developer.nvidia.com/blog/inside-nvidia-groq-3-lpx-the-low-latency-inference-accelerator-for-the-nvidia-vera-rubin-platform/)。

边界：公开能力用owned放大示意说明；不声称供应商physical floorplan、逐周期RTL、真实工艺比例或测量。

### speculative-decoding

draft→verify→accept/reject/rollback

要讲清楚：多draft tokens；target verify结果；accepted prefix与rejected suffix回退。

素材ID：`prefill-decode-split`。

镜头：[39-prefill-decode-split](SHOTS.md#39-prefill-decode-split)。

原章节：lpx:08.2。

近景：[main-structure-detail](previews/prefill-decode-split/main-structure-detail.jpg) · [top](previews/prefill-decode-split/top.jpg) · [hero](previews/prefill-decode-split/hero.jpg)。

依据：[Inside NVIDIA Groq 3 LPX](https://developer.nvidia.com/blog/inside-nvidia-groq-3-lpx-the-low-latency-inference-accelerator-for-the-nvidia-vera-rubin-platform/)。

边界：公开能力用owned放大示意说明；不声称供应商physical floorplan、逐周期RTL、真实工艺比例或测量。

### roofline-intensity

Roofline、batch/data reuse与带宽瓶颈

要讲清楚：operations/byte横轴；bandwidth斜线与compute水平上限；batch变化的工作点。

素材ID：`roofline-batch-intensity`, `gpu-tensor-dataflow`, `prefill-decode-split`。

镜头：[54-roofline-batch-intensity](SHOTS.md#54-roofline-batch-intensity), [34-gpu-tensor-dataflow](SHOTS.md#34-gpu-tensor-dataflow)。

原章节：lpx:03.3, lpx:05.2。

近景：[main-structure-detail](previews/roofline-batch-intensity/main-structure-detail.jpg) · [top](previews/roofline-batch-intensity/top.jpg) · [hero](previews/roofline-batch-intensity/hero.jpg)。

依据：[Roofline visual performance model author paper, revised2008](https://people.eecs.berkeley.edu/~kubitron/courses/cs252/handouts/papers/RooflineVyNoYellow.pdf)。

边界：公开能力用owned放大示意说明；不声称供应商physical floorplan、逐周期RTL、真实工艺比例或测量。

### distributed-sram-capacity

把SRAM分布到多LPU/wafer tile的容量与路由取舍

要讲清楚：local bank容量；multi-chip/tile route；总容量不等同任何core的local cache。

素材ID：`memory-hierarchy`, `lpu-c2c-network`, `gpu-tensor-dataflow`。

镜头：[38-lpu-c2c-network](SHOTS.md#38-lpu-c2c-network), [34-gpu-tensor-dataflow](SHOTS.md#34-gpu-tensor-dataflow), [29-memory-hierarchy](SHOTS.md#29-memory-hierarchy)。

原章节：lpx:05.3-05.4, lpx:11.1。

近景：[main-structure-detail](previews/memory-hierarchy/main-structure-detail.jpg) · [top](previews/memory-hierarchy/top.jpg) · [hero](previews/memory-hierarchy/hero.jpg)。

依据：[MIT6.004: memory cells, cache lookup and generic coherence principles](https://ocw.mit.edu/courses/6-004-computation-structures-spring-2017/pages/c14/c14s1/) · [Inside NVIDIA Groq 3 LPX](https://developer.nvidia.com/blog/inside-nvidia-groq-3-lpx-the-low-latency-inference-accelerator-for-the-nvidia-vera-rubin-platform/)。

边界：8C聚合不等于一核心local CL；C到CL线表达子域关系而非厂商布线。

### vrm-pdn-decap

VRM、inductor/decap与负载di/dt droop

要讲清楚：load电流step；decap先供电/VRM跟上；电压droop示意，非精确波形。

素材ID：`power-vrm-pdn`。

镜头：[56-power-vrm-pdn](SHOTS.md#56-power-vrm-pdn)。

原章节：lpx:09.1, nvl72:07.3。

近景：[main-structure-detail](previews/power-vrm-pdn/main-structure-detail.jpg) · [functional-vrm-phase0](previews/power-vrm-pdn/functional-vrm-phase0.jpg) · [assembled-detail](previews/power-vrm-pdn/assembled-detail.jpg)。

依据：[Groq3LPX deterministic execution and proactive power control](https://developer.nvidia.com/blog/how-nvidia-groq-3-lpx-deterministic-execution-drives-power-efficient-high-interactivity-inference-on-nvidia-vera-rubin/) · [TI SLVA882B: Multiphase Buck Design From Start to Finish](https://www.ti.com/lit/an/slva882b/slva882b.pdf)。

边界：multiphase buck generic拓扑；HS/LS死区和diode续流是状态示意，无电路求解。

### lpu-pep-cps

PEP提前PDN命令与CPS变化周期

要讲清楚：compiler预测current；PEP提前raise supply；CPS拉长危险cycle降低di/dt；两机制独立。

素材ID：`power-smoothing`, `power-vrm-pdn`, `lpu-static-schedule`。

镜头：[57-power-smoothing](SHOTS.md#57-power-smoothing), [37-lpu-static-schedule](SHOTS.md#37-lpu-static-schedule)。

原章节：lpx:09.2-09.3。

近景：[functional-timing-detail-pep-comparison](previews/power-smoothing/functional-timing-detail-pep-comparison.jpg) · [functional-timing-detail-cps-comparison](previews/power-smoothing/functional-timing-detail-cps-comparison.jpg) · [main-structure-detail](previews/power-smoothing/main-structure-detail.jpg)。

依据：[Groq3LPX deterministic execution and proactive power control](https://developer.nvidia.com/blog/how-nvidia-groq-3-lpx-deterministic-execution-drives-power-efficient-high-interactivity-inference-on-nvidia-vera-rubin/)。

边界：CMD/I/V分别表示；normalized周期延长不是Groq实测电压/时延。

### wafer-systolic-topology

wafer-tiled SRAM与TPU式systolic/torus对照

要讲清楚：generic tiled SRAM+compute；邻居MAC逐拍流动；torus wrap edges和mesh/switch对照。

素材ID：`gpu-tensor-dataflow`, `memory-hierarchy`, `lpu-c2c-network`。

镜头：[34-gpu-tensor-dataflow](SHOTS.md#34-gpu-tensor-dataflow), [38-lpu-c2c-network](SHOTS.md#38-lpu-c2c-network)。

原章节：lpx:11.1-11.2。

近景：[main-structure-detail](previews/gpu-tensor-dataflow/main-structure-detail.jpg) · [functional-timing-detail-generic-topology-comparator](previews/gpu-tensor-dataflow/functional-timing-detail-generic-topology-comparator.jpg) · [top](previews/gpu-tensor-dataflow/top.jpg)。

依据：[MIT6.004: memory cells, cache lookup and generic coherence principles](https://ocw.mit.edu/courses/6-004-computation-structures-spring-2017/pages/c14/c14s1/) · [Roofline visual performance model author paper, revised2008](https://people.eecs.berkeley.edu/~kubitron/courses/cs252/handouts/papers/RooflineVyNoYellow.pdf)。

边界：generic wafer tile/3×3 torus明确NOT GROQ/NOT RUBIN FLOORPLAN，不声称vendor节点数。

## BlueField-4 STX / CMX

### nand-trap-channel

3D NAND垂直channel/charge trap

要讲清楚：vertical channel；tunnel/trap/blocking dielectric；wordline、charge injection与read current。

素材ID：`nand-charge-trap`。

镜头：[30-nand-charge-trap](SHOTS.md#30-nand-charge-trap)。

原章节：stx:05.1。

近景：[main-structure-detail](previews/nand-charge-trap/main-structure-detail.jpg) · [functional-single-cell-section](previews/nand-charge-trap/functional-single-cell-section.jpg) · [top](previews/nand-charge-trap/top.jpg)。

依据：[3D Flash Memory charge-trap program and erase mechanism](https://www.kioxia.com/en-jp/rd/technology/topics/topics-88.html)。

边界：公开能力用owned放大示意说明；不声称供应商physical floorplan、逐周期RTL、真实工艺比例或测量。

### nand-threshold-levels

TLC/QLC阈值分布与密度裕量

要讲清楚：8与16state；programmed voltage windows；read threshold与margin；不画实测分布。

素材ID：`nand-threshold-levels`。

镜头：[31-nand-threshold-levels](SHOTS.md#31-nand-threshold-levels)。

原章节：stx:05.2。

近景：[main-structure-detail](previews/nand-threshold-levels/main-structure-detail.jpg) · [top](previews/nand-threshold-levels/top.jpg) · [hero](previews/nand-threshold-levels/hero.jpg)。

依据：[QLC versus TLC flash storage technology](https://blog-us.kioxia.com/post/2026/09/29/qlc-vs-tlc-flash-storage-technology-how-to-choose)。

边界：此SLC=Single-Level Cell、每cell1bit；不同于Vera System-Level Cache。分布间距不是实测。

### ssd-ftl-gc

SSD channel/FTL/page relocation/GC

要讲清楚：logical page映射physical page；valid/invalid data移动；block erase与额外write，非固件复刻。

素材ID：`ssd-controller-ftl`。

镜头：[32-ssd-controller-ftl](SHOTS.md#32-ssd-controller-ftl)。

原章节：stx:05.3-05.4。

近景：[main-structure-detail](previews/ssd-controller-ftl/main-structure-detail.jpg) · [functional-processor-wear](previews/ssd-controller-ftl/functional-processor-wear.jpg) · [top](previews/ssd-controller-ftl/top.jpg)。

依据：[Erase overhead in low-latency SSDs](https://www.kioxia.com/en-jp/rd/technology/topics/topics-51.html) · [Understanding Wear Leveling in NAND Flash Memory](https://www.kioxia.com/content/dam/kioxia/shared/business/memory/mlc-nand/asset/productbrief/KIOXIA_Understanding_Wear_Leveling_Tech_Brief.pdf)。

边界：公开能力用owned放大示意说明；不声称供应商physical floorplan、逐周期RTL、真实工艺比例或测量。

### ssd-wear-ecc

SSD endurance、wear leveling与ECC

要讲清楚：不同erase counts；valid data迁移；纠错/校验与重试角色。

素材ID：`ssd-controller-ftl`。

镜头：[32-ssd-controller-ftl](SHOTS.md#32-ssd-controller-ftl)。

原章节：stx:05.3-05.5。

近景：[main-structure-detail](previews/ssd-controller-ftl/main-structure-detail.jpg) · [functional-processor-erasure-recover](previews/ssd-controller-ftl/functional-processor-erasure-recover.jpg) · [functional-processor-ecc-retry](previews/ssd-controller-ftl/functional-processor-ecc-retry.jpg)。

依据：[Understanding Wear Leveling in NAND Flash Memory](https://www.kioxia.com/content/dam/kioxia/shared/business/memory/mlc-nand/asset/productbrief/KIOXIA_Understanding_Wear_Leveling_Tech_Brief.pdf) · [Erase overhead in low-latency SSDs](https://www.kioxia.com/en-jp/rd/technology/topics/topics-51.html) · [MIT6.02: linear block codes and syndrome decoding](https://ocw.mit.edu/courses/6-02-introduction-to-eecs-ii-digital-communication-systems-fall-2012/34b7d78e0b90235095ef81542f6aa2dc_MIT6_02F12_chap06.pdf)。

边界：toy Hamming/GF、retry与擦除计数；不冒充量产SSD ECC码或寿命模型。

### kv-tensor-size

KV为attention中间tensor与容量变化

要讲清楚：K/V两组tensor；layers/heads/sequence/batch/precision可调概念；聊天文本不等于KVtensor。

素材ID：`kv-cache-tiers`, `prefill-decode-split`。

镜头：[33-kv-cache-tiers](SHOTS.md#33-kv-cache-tiers), [39-prefill-decode-split](SHOTS.md#39-prefill-decode-split)。

原章节：stx:01.1-01.3。

近景：[functional-kv-tensor](previews/kv-cache-tiers/functional-kv-tensor.jpg) · [main-structure-detail](previews/kv-cache-tiers/main-structure-detail.jpg) · [top](previews/kv-cache-tiers/top.jpg)。

依据：[Introducing BlueField-4-powered CMX context memory storage](https://developer.nvidia.com/blog/introducing-nvidia-bluefield-4-powered-inference-context-memory-storage-platform-for-the-next-frontier-of-ai/)。

边界：公开能力用owned放大示意说明；不声称供应商physical floorplan、逐周期RTL、真实工艺比例或测量。

### kv-prestage-reuse

G1/G2/G3/G3.5/G4迁移、预取与复用

要讲清楚：G3.5Ethernetflash位置；prefetch→near memory→decode；reuse identity/model/tenant约束，非文本相同即可复用。

素材ID：`kv-cache-tiers`, `memory-hierarchy`。

镜头：[33-kv-cache-tiers](SHOTS.md#33-kv-cache-tiers)。

原章节：stx:06.1-06.5, stx:07。

近景：[main-structure-detail](previews/kv-cache-tiers/main-structure-detail.jpg) · [functional-processor-kv-identity](previews/kv-cache-tiers/functional-processor-kv-identity.jpg) · [functional-processor-kv-reuse-miss](previews/kv-cache-tiers/functional-processor-kv-reuse-miss.jpg)。

依据：[Introducing BlueField-4-powered CMX context memory storage](https://developer.nvidia.com/blog/introducing-nvidia-bluefield-4-powered-inference-context-memory-storage-platform-for-the-next-frontier-of-ai/)。

边界：公开能力用owned放大示意说明；不声称供应商physical floorplan、逐周期RTL、真实工艺比例或测量。

### nixl-memos-dynamo

Dynamo策略、NIXL传输、DOCA存储路径

要讲清楚：policy与transport分层；KV transfer方向；driver/controller上下文。

素材ID：`kv-cache-tiers`, `rdma-astra-data-path`。

镜头：[33-kv-cache-tiers](SHOTS.md#33-kv-cache-tiers)。

原章节：stx:06.3-06.4。

近景：[functional-processor-kv-identity](previews/kv-cache-tiers/functional-processor-kv-identity.jpg) · [functional-processor-kv-reuse-miss](previews/kv-cache-tiers/functional-processor-kv-reuse-miss.jpg) · [functional-processor-kv-placement](previews/kv-cache-tiers/functional-processor-kv-placement.jpg)。

依据：[Introducing BlueField-4-powered CMX context memory storage](https://developer.nvidia.com/blog/introducing-nvidia-bluefield-4-powered-inference-context-memory-storage-platform-for-the-next-frontier-of-ai/) · [Dynamo1.2.0 KV Block Manager architecture](https://docs.nvidia.com/dynamo/v1.2.0/components/kvbm) · [NVIDIA CMX product documentation: DOCA Memos SDK and software roles](https://www.nvidia.com/en-us/data-center/ai-storage/cmx/)。

边界：Dynamo策略、NIXL注册搬运与DOCA Memos SDK服务CMX；不是独立MemOS软件。

### cxl-vs-cmx

CXL load/store内存扩展对照Ethernet NVMe flash

要讲清楚：memory coherence/load-store路径；RDMA/storage command路径；DRAM与persistent NAND分别可见。

素材ID：`cxl-vs-cmx`。

镜头：[51-cxl-vs-cmx](SHOTS.md#51-cxl-vs-cmx)。

原章节：stx:08.2, vera:05.3。

近景：[main-structure-detail](previews/cxl-vs-cmx/main-structure-detail.jpg) · [top](previews/cxl-vs-cmx/top.jpg) · [hero](previews/cxl-vs-cmx/hero.jpg)。

依据：[NVIDIA Vera CPU Architecture Whitepaper v1.12](https://nvdam.nvidia.com/Share/qkf77fo0u75m4o03ifxkae0a151h2b6k) · [Introducing BlueField-4-powered CMX context memory storage](https://developer.nvidia.com/blog/introducing-nvidia-bluefield-4-powered-inference-context-memory-storage-platform-for-the-next-frontier-of-ai/) · [CXL Consortium: coherent memory and host load/store semantics](https://computeexpresslink.org/blog/questions-from-the-compute-express-link-exploring-coherent-memory-and-innovative-use-cases-webinar-2341/)。

边界：CXL load/store与支持域的一致性；CMX是Ethernet KV flash/API，不扩成任意GPU全局一致内存。

### storage-offload

CRC/压缩/AES/erasure-code offload链路

要讲清楚：payload分块；integrity/encryption/恢复角色；network→processor→SSD。

素材ID：`rdma-astra-data-path`, `ssd-controller-ftl`, `chip-bf4-stx`, `chip-bf4-dpu`。

镜头：[32-ssd-controller-ftl](SHOTS.md#32-ssd-controller-ftl), [42-rdma-astra-data-path](SHOTS.md#42-rdma-astra-data-path), [19-chip-bf4-dpu](SHOTS.md#19-chip-bf4-dpu)。

原章节：stx:04.2-04.4。

近景：[functional-processor-bf4-control](previews/rdma-astra-data-path/functional-processor-bf4-control.jpg) · [main-structure-detail](previews/rdma-astra-data-path/main-structure-detail.jpg) · [top](previews/rdma-astra-data-path/top.jpg)。

依据：[Scaling agentic AI factories with NVIDIA BlueField](https://developer.nvidia.com/blog/scaling-agentic-ai-factories-through-extreme-co-design-with-nvidia-bluefield/) · [NVIDIA Vera CPU Architecture Whitepaper v1.12](https://nvdam.nvidia.com/Share/qkf77fo0u75m4o03ifxkae0a151h2b6k) · [Vera storage benchmarks: encryption, compression, integrity checking and recovery](https://developer.nvidia.com/blog/nvidia-vera-storage-benchmarks-faster-encryption-compression-integrity-checking-and-recovery-for-ai-native-storage/) · [NIST FIPS197: Advanced Encryption Standard](https://csrc.nist.gov/pubs/fips/197/final) · [NIST AES-128 core example: public ECB round trace](https://csrc.nist.gov/CSRC/media/Projects/Cryptographic-Standards-and-Guidelines/documents/examples/AES_Core128.pdf) · [RFC3720: CRC32C digest definition and examples](https://datatracker.ietf.org/doc/html/rfc3720)。

边界：公开offload角色+明确字节/CRC/AES/LZ/GF教材例；不是具体厂商加速器数量/量产码流。

## Spectrum-6 SPX / CPO

### channel-equalization

损耗/反射/ISI与FFE/CTLE/DFE

要讲清楚：原始/受损波形；CTLE/FFE与past-decision反馈；equalized eye与误判。

素材ID：`serdes-equalization-cdr`。

镜头：[46-serdes-equalization-cdr](SHOTS.md#46-serdes-equalization-cdr)。

原章节：spx:03.2-03.3。

近景：[main-structure-detail](previews/serdes-equalization-cdr/main-structure-detail.jpg) · [top](previews/serdes-equalization-cdr/top.jpg) · [hero](previews/serdes-equalization-cdr/hero.jpg)。

依据：[SNLA401: redriver and retimer signal conditioning](https://www.ti.com/document-viewer/lit/html/SNLA401) · [DS560DF810 56Gbps multirate retimer datasheet RevB](https://www.ti.com/lit/ds/symlink/ds560df810.pdf)。

边界：公开能力用owned放大示意说明；不声称供应商physical floorplan、逐周期RTL、真实工艺比例或测量。

### cdr-loop

CDR phase detector/filter/clock与采样

要讲清楚：phase error反馈；recovered clock；sample位置移动。

素材ID：`serdes-equalization-cdr`。

镜头：[46-serdes-equalization-cdr](SHOTS.md#46-serdes-equalization-cdr)。

原章节：spx:03.3。

近景：[main-structure-detail](previews/serdes-equalization-cdr/main-structure-detail.jpg) · [functional-cdr-sampling](previews/serdes-equalization-cdr/functional-cdr-sampling.jpg) · [top](previews/serdes-equalization-cdr/top.jpg)。

依据：[SNLA401: redriver and retimer signal conditioning](https://www.ti.com/document-viewer/lit/html/SNLA401) · [DS560DF810 56Gbps multirate retimer datasheet RevB](https://www.ti.com/lit/ds/symlink/ds560df810.pdf)。

边界：公开能力用owned放大示意说明；不声称供应商physical floorplan、逐周期RTL、真实工艺比例或测量。

### multiplane-shuffle

independent planes、rail与fiber shuffle

要讲清楚：NIC到多plane连接；坏plane被mask；四ASICinternal fiber shuffle不同于额外光交换。

素材ID：`network-multiplane`, `switch-sn6800`。

镜头：[50-network-multiplane](SHOTS.md#50-network-multiplane), [13-switch-sn6800](SHOTS.md#13-switch-sn6800)。

原章节：spx:01.2, spx:08.3。

近景：[main-structure-detail](previews/network-multiplane/main-structure-detail.jpg) · [top](previews/network-multiplane/top.jpg) · [hero](previews/network-multiplane/hero.jpg)。

依据：[Giga-scale Spectrum-X Ethernet and multiplane networking](https://developer.nvidia.com/blog/giga-scale-ai-ethernet-evolution-spectrum-x-ethernet-rewrites-rules/) · [NVIDIA Spectrum-6 SN6000 Switch Systems Hardware User Manual 1.3](https://networking-docs.nvidia.com/sn6000hw/1.3/specifications)。

边界：公开能力用owned放大示意说明；不声称供应商physical floorplan、逐周期RTL、真实工艺比例或测量。

### els-cw-modulate

ELS→CW input→EIC驱动PIC→data output

要讲清楚：ELS激光泵浦单独路径；CW与data方向/颜色区分；ASIC电bit进入EIC再调制。

素材ID：`cpo-engine`, `photonics-microring`。

镜头：[23-cpo-engine](SHOTS.md#23-cpo-engine), [47-photonics-microring](SHOTS.md#47-photonics-microring)。

原章节：spx:04.3, spx:07.1。

近景：[assembled-detail](previews/cpo-engine/assembled-detail.jpg) · [service-detail](previews/cpo-engine/service-detail.jpg) · [pcb-detail](previews/cpo-engine/pcb-detail.jpg)。

依据：[NVIDIA silicon photonics-based network switching](https://developer.nvidia.com/blog/a-new-era-in-data-center-networking-with-nvidia-silicon-photonics-based-network-switching/) · [How industry collaboration fosters NVIDIA co-packaged optics](https://developer.nvidia.com/blog/how-industry-collaboration-fosters-nvidia-co-packaged-optics/)。

边界：CW持续供光；电数据驱动MRM，再把调制光送TX纤，光点不是光场求解。

### microring-tuning

微环evanescent coupling、PN调制与thermal tuning

要讲清楚：bus waveguide紧邻ring；电极改变折射率；heater温调与数据调制分角色。

素材ID：`photonics-microring`, `cpo-engine`。

镜头：[47-photonics-microring](SHOTS.md#47-photonics-microring), [23-cpo-engine](SHOTS.md#23-cpo-engine)。

原章节：spx:05.1-05.3。

近景：[main-structure-detail](previews/photonics-microring/main-structure-detail.jpg) · [top](previews/photonics-microring/top.jpg) · [hero](previews/photonics-microring/hero.jpg)。

依据：[How industry collaboration fosters NVIDIA co-packaged optics](https://developer.nvidia.com/blog/how-industry-collaboration-fosters-nvidia-co-packaged-optics/) · [NVIDIA silicon photonics-based network switching](https://developer.nvidia.com/blog/a-new-era-in-data-center-networking-with-nvidia-silicon-photonics-based-network-switching/)。

边界：公开能力用owned放大示意说明；不声称供应商physical floorplan、逐周期RTL、真实工艺比例或测量。

### receive-pd-tia

RX optical→photodiode current→TIA voltage

要讲清楚：RX fiber入光；PD与EIC内TIA分别可见；输出电信号回ASIC；专利不等同量产认证。

素材ID：`cpo-engine`, `cpo-package-section`。

镜头：[23-cpo-engine](SHOTS.md#23-cpo-engine), [49-cpo-package-section](SHOTS.md#49-cpo-package-section)。

原章节：spx:04.3。

近景：[assembled-detail](previews/cpo-engine/assembled-detail.jpg) · [service-detail](previews/cpo-engine/service-detail.jpg) · [pcb-detail](previews/cpo-engine/pcb-detail.jpg)。

依据：[US12618712B2 Differential transimpedance amplifier from a single photodiode](https://patents.google.com/patent/US12618712B2/en)。

边界：RX photons→PD current→TIA voltage后为电路径，不把PD到TIA画成继续传光。

### eic-pic-package

EIC/PIC3D hybrid bond与package section

要讲清楚：EIC/PIC不同silicon层；细电bond垂直连接；optical coupling与电bond分开。

素材ID：`cpo-package-section`, `chip-spectrum`, `cpo-engine`。

镜头：[49-cpo-package-section](SHOTS.md#49-cpo-package-section), [23-cpo-engine](SHOTS.md#23-cpo-engine)。

原章节：spx:06.1-06.3。

近景：[main-structure-detail](previews/cpo-package-section/main-structure-detail.jpg) · [functional-cpo-bond-section](previews/cpo-package-section/functional-cpo-bond-section.jpg) · [functional-package-comparison](previews/cpo-package-section/functional-package-comparison.jpg)。

依据：[How industry collaboration fosters NVIDIA co-packaged optics](https://developer.nvidia.com/blog/how-industry-collaboration-fosters-nvidia-co-packaged-optics/)。

边界：共面Cu/dielectric的generic hybrid bond揭示；不是厂商真实mask或接触/良率检查。

### laser-architecture-options

external ELS与集成laser/SOA比较

要讲清楚：外部serviceable laser；集成laser与PIC；波长/功率分配；Intel2024prototype上下文。

素材ID：`photonics-laser-options`。

镜头：[48-photonics-laser-options](SHOTS.md#48-photonics-laser-options)。

原章节：spx:07.1, spx:09.3。

近景：[main-structure-detail](previews/photonics-laser-options/main-structure-detail.jpg) · [top](previews/photonics-laser-options/top.jpg) · [hero](previews/photonics-laser-options/hero.jpg)。

依据：[NVIDIA silicon photonics-based network switching](https://developer.nvidia.com/blog/a-new-era-in-data-center-networking-with-nvidia-silicon-photonics-based-network-switching/) · [Intel fully integrated optical IO chiplet demonstration](https://www.intel.com/content/www/us/en/newsroom/news/intel-unveils-first-integrated-optical-io-chiplet.html)。

边界：外ELS为NVIDIA公开结构；集成gain对照来自Intel OCI原型，非NVIDIA量产断言。

### optical-channel-link-budget

光纤coupler、loss与传播time

要讲清楚：fiber→coupler→waveguide边界；光功率逐段预算；有限传播时延，不混22dB电损耗。

素材ID：`cpo-engine`, `photonics-laser-options`。

镜头：[48-photonics-laser-options](SHOTS.md#48-photonics-laser-options), [23-cpo-engine](SHOTS.md#23-cpo-engine)。

原章节：spx:06.2, spx:07.2-07.3。

近景：[assembled-detail](previews/cpo-engine/assembled-detail.jpg) · [service-detail](previews/cpo-engine/service-detail.jpg) · [pcb-detail](previews/cpo-engine/pcb-detail.jpg)。

依据：[How industry collaboration fosters NVIDIA co-packaged optics](https://developer.nvidia.com/blog/how-industry-collaboration-fosters-nvidia-co-packaged-optics/) · [Intel fully integrated optical IO chiplet demonstration](https://www.intel.com/content/www/us/en/newsroom/news/intel-unveils-first-integrated-optical-io-chiplet.html)。

边界：dBm功率−dB损耗与ngL/c，柱高另为normalized相对功率；不是实测链路budget。

### mzm-vs-mrm

MZM两臂干涉与MRM谐振比较

要讲清楚：MZM两臂/重合输出；ring resonance对照；通用机制不声称S6替代布局。

素材ID：`photonics-microring`。

镜头：[47-photonics-microring](SHOTS.md#47-photonics-microring)。

原章节：spx:05.4。

近景：[functional-mzm-comparator](previews/photonics-microring/functional-mzm-comparator.jpg) · [main-structure-detail](previews/photonics-microring/main-structure-detail.jpg) · [top](previews/photonics-microring/top.jpg)。

依据：[How industry collaboration fosters NVIDIA co-packaged optics](https://developer.nvidia.com/blog/how-industry-collaboration-fosters-nvidia-co-packaged-optics/) · [Ansys traveling-wave Mach-Zehnder modulator example and 2x2 compact model](https://optics.ansys.com/hc/en-us/articles/360042328774-Traveling-Wave-Mach-Zehnder-Modulator)。

边界：Y splitter→双arm phase→recombiner与微环谐振比较；未计算干涉场/谱。
