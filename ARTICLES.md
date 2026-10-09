# 五篇Rubin内容的现有选材

从叙事问题选择素材，再用镜头阶段表确定剪辑区间。同一资产可跨篇复用。

## Vera Rubin NVL72

一套GPU超级计算机怎样从机房连接到芯片内部？

可用顺序：01→02→07→16→22→28；按需要插入34、40、41、53、54、55、56。

主归属29个讲解点；交叉关联53项资产、43组镜头。

讲解点：`assembly-hierarchy`, `tray-midplane`, `rubin-chiplet`, `tensor-mac`, `nvfp4-format`, `hbm-dram-stack`, `hbm-tsv-bumps`, `hbm-interposer`, `hbm-parallel-interface`, `dram1t1c`, `numa-c2c-coherence`, `spatial-multithreading`, `socamm-compression`, `mesh-vs-switched`, `passive-copper-spine`, `sharp-reduction`, `rdma-gpudirect`, `rdma-registration-protection`, `astra-control-data-domains`, `packet-pipeline`, `queue-hol-incast`, `ar-tcc-plb`, `osfp-vs-cpo`, `liquid-heat-path`, `liquid-qd-service`, `busbar-power-path`, `vrm-pdn-decap`, `rack-power-smoothing`, `ras-repair-maintenance`, `package-comparison-principles`。

镜头：[01-pod-tour](SHOTS.md#01-pod-tour), [02-rack-nvl72](SHOTS.md#02-rack-nvl72), [03-rack-vera](SHOTS.md#03-rack-vera), [04-rack-lpx](SHOTS.md#04-rack-lpx), [05-rack-stx](SHOTS.md#05-rack-stx), [06-rack-spx](SHOTS.md#06-rack-spx), [07-tray-compute](SHOTS.md#07-tray-compute), [08-tray-nvlink](SHOTS.md#08-tray-nvlink), [09-tray-vera](SHOTS.md#09-tray-vera), [10-tray-lpx](SHOTS.md#10-tray-lpx), [11-tray-stx](SHOTS.md#11-tray-stx), [12-tray-etl](SHOTS.md#12-tray-etl), [13-switch-sn6800](SHOTS.md#13-switch-sn6800), [14-switch-sn6810](SHOTS.md#14-switch-sn6810), [15-chip-vera](SHOTS.md#15-chip-vera), [16-chip-rubin](SHOTS.md#16-chip-rubin), [17-chip-nvlink](SHOTS.md#17-chip-nvlink), [18-chip-cx9](SHOTS.md#18-chip-cx9), [19-chip-bf4-dpu](SHOTS.md#19-chip-bf4-dpu), [20-chip-groq](SHOTS.md#20-chip-groq), [21-chip-spectrum](SHOTS.md#21-chip-spectrum), [22-hbm4-section](SHOTS.md#22-hbm4-section), [23-cpo-engine](SHOTS.md#23-cpo-engine), [24-pod-to-die](SHOTS.md#24-pod-to-die), [26-memory-cell-dram1t1c](SHOTS.md#26-memory-cell-dram1t1c), [27-memory-cell-comparison](SHOTS.md#27-memory-cell-comparison), [28-hbm4-tsv](SHOTS.md#28-hbm4-tsv), [34-gpu-tensor-dataflow](SHOTS.md#34-gpu-tensor-dataflow), [35-cpu-olympus-pipeline](SHOTS.md#35-cpu-olympus-pipeline), [36-cpu-scf-coherence](SHOTS.md#36-cpu-scf-coherence), [38-lpu-c2c-network](SHOTS.md#38-lpu-c2c-network), [40-network-mesh-fabric](SHOTS.md#40-network-mesh-fabric), [41-network-sharp-reduction](SHOTS.md#41-network-sharp-reduction), [42-rdma-astra-data-path](SHOTS.md#42-rdma-astra-data-path), [43-switch-packet-pipeline](SHOTS.md#43-switch-packet-pipeline), [44-network-incast-control](SHOTS.md#44-network-incast-control), [45-serdes-pam4](SHOTS.md#45-serdes-pam4), [49-cpo-package-section](SHOTS.md#49-cpo-package-section), [50-network-multiplane](SHOTS.md#50-network-multiplane), [53-nvfp4-block-scaling](SHOTS.md#53-nvfp4-block-scaling), [55-liquid-cooling-section](SHOTS.md#55-liquid-cooling-section), [56-power-vrm-pdn](SHOTS.md#56-power-vrm-pdn), [57-power-smoothing](SHOTS.md#57-power-smoothing)。

## Vera CPU Rack

CPU为什么仍是智能体工厂的关键，核心、缓存和内存怎样配合？

可用顺序：03→09→15→35→36→52；用SOCAMM2近景以及45/46/51补充接口与内存路径。

主归属14个讲解点；交叉关联45项资产、35组镜头。

讲解点：`assembly-hierarchy`, `memory-hierarchy`, `cache-array-banks`, `numa-c2c-coherence`, `vera-io-phy-bifurcation`, `olympus-front-end`, `branch-predictor`, `ooo-rename-commit`, `memory-rename-value-prediction`, `graph-prefetch`, `spatial-multithreading`, `scf-nodes-slcs`, `coherence-state`, `socamm-compression`, `agent-cpu-gpu-loop`, `passive-copper-spine`, `astra-control-data-domains`, `pcs-fec`, `pam4-nrz`, `ar-tcc-plb`, `cxl-vs-cmx`, `confidential-domains`, `liquid-heat-path`, `liquid-qd-service`, `ras-repair-maintenance`, `package-comparison-principles`。

镜头：[01-pod-tour](SHOTS.md#01-pod-tour), [02-rack-nvl72](SHOTS.md#02-rack-nvl72), [03-rack-vera](SHOTS.md#03-rack-vera), [04-rack-lpx](SHOTS.md#04-rack-lpx), [05-rack-stx](SHOTS.md#05-rack-stx), [06-rack-spx](SHOTS.md#06-rack-spx), [07-tray-compute](SHOTS.md#07-tray-compute), [08-tray-nvlink](SHOTS.md#08-tray-nvlink), [09-tray-vera](SHOTS.md#09-tray-vera), [10-tray-lpx](SHOTS.md#10-tray-lpx), [11-tray-stx](SHOTS.md#11-tray-stx), [12-tray-etl](SHOTS.md#12-tray-etl), [13-switch-sn6800](SHOTS.md#13-switch-sn6800), [14-switch-sn6810](SHOTS.md#14-switch-sn6810), [15-chip-vera](SHOTS.md#15-chip-vera), [16-chip-rubin](SHOTS.md#16-chip-rubin), [19-chip-bf4-dpu](SHOTS.md#19-chip-bf4-dpu), [24-pod-to-die](SHOTS.md#24-pod-to-die), [28-hbm4-tsv](SHOTS.md#28-hbm4-tsv), [29-memory-hierarchy](SHOTS.md#29-memory-hierarchy), [33-kv-cache-tiers](SHOTS.md#33-kv-cache-tiers), [35-cpu-olympus-pipeline](SHOTS.md#35-cpu-olympus-pipeline), [36-cpu-scf-coherence](SHOTS.md#36-cpu-scf-coherence), [37-lpu-static-schedule](SHOTS.md#37-lpu-static-schedule), [38-lpu-c2c-network](SHOTS.md#38-lpu-c2c-network), [39-prefill-decode-split](SHOTS.md#39-prefill-decode-split), [42-rdma-astra-data-path](SHOTS.md#42-rdma-astra-data-path), [44-network-incast-control](SHOTS.md#44-network-incast-control), [45-serdes-pam4](SHOTS.md#45-serdes-pam4), [46-serdes-equalization-cdr](SHOTS.md#46-serdes-equalization-cdr), [49-cpo-package-section](SHOTS.md#49-cpo-package-section), [50-network-multiplane](SHOTS.md#50-network-multiplane), [51-cxl-vs-cmx](SHOTS.md#51-cxl-vs-cmx), [52-cpu-graph-prefetch](SHOTS.md#52-cpu-graph-prefetch), [55-liquid-cooling-section](SHOTS.md#55-liquid-cooling-section)。

## Groq 3 LPX

为什么另一种加速器用片上SRAM与静态排时追求低延迟？

可用顺序：04→10→20→25/26/27→37→38→39→54→57。

主归属16个讲解点；交叉关联41项资产、35组镜头。

讲解点：`assembly-hierarchy`, `tensor-mac`, `hbm-dram-stack`, `hbm-tsv-bumps`, `sram6t`, `dram1t1c`, `cell-structure-comparison`, `memory-hierarchy`, `cache-array-banks`, `lpu-functional-engines`, `static-schedule`, `lpu-bank-conflicts`, `plesiosynchronous-clock`, `lpu-direct-c2c`, `lpu-fel-dram`, `prefill-decode`, `attention-ffn`, `speculative-decoding`, `roofline-intensity`, `distributed-sram-capacity`, `liquid-heat-path`, `vrm-pdn-decap`, `lpu-pep-cps`, `package-comparison-principles`, `wafer-systolic-topology`。

镜头：[01-pod-tour](SHOTS.md#01-pod-tour), [02-rack-nvl72](SHOTS.md#02-rack-nvl72), [03-rack-vera](SHOTS.md#03-rack-vera), [04-rack-lpx](SHOTS.md#04-rack-lpx), [05-rack-stx](SHOTS.md#05-rack-stx), [06-rack-spx](SHOTS.md#06-rack-spx), [07-tray-compute](SHOTS.md#07-tray-compute), [08-tray-nvlink](SHOTS.md#08-tray-nvlink), [09-tray-vera](SHOTS.md#09-tray-vera), [10-tray-lpx](SHOTS.md#10-tray-lpx), [11-tray-stx](SHOTS.md#11-tray-stx), [12-tray-etl](SHOTS.md#12-tray-etl), [13-switch-sn6800](SHOTS.md#13-switch-sn6800), [14-switch-sn6810](SHOTS.md#14-switch-sn6810), [15-chip-vera](SHOTS.md#15-chip-vera), [16-chip-rubin](SHOTS.md#16-chip-rubin), [20-chip-groq](SHOTS.md#20-chip-groq), [22-hbm4-section](SHOTS.md#22-hbm4-section), [24-pod-to-die](SHOTS.md#24-pod-to-die), [25-memory-cell-sram6t](SHOTS.md#25-memory-cell-sram6t), [26-memory-cell-dram1t1c](SHOTS.md#26-memory-cell-dram1t1c), [27-memory-cell-comparison](SHOTS.md#27-memory-cell-comparison), [28-hbm4-tsv](SHOTS.md#28-hbm4-tsv), [29-memory-hierarchy](SHOTS.md#29-memory-hierarchy), [33-kv-cache-tiers](SHOTS.md#33-kv-cache-tiers), [34-gpu-tensor-dataflow](SHOTS.md#34-gpu-tensor-dataflow), [36-cpu-scf-coherence](SHOTS.md#36-cpu-scf-coherence), [37-lpu-static-schedule](SHOTS.md#37-lpu-static-schedule), [38-lpu-c2c-network](SHOTS.md#38-lpu-c2c-network), [39-prefill-decode-split](SHOTS.md#39-prefill-decode-split), [49-cpo-package-section](SHOTS.md#49-cpo-package-section), [54-roofline-batch-intensity](SHOTS.md#54-roofline-batch-intensity), [55-liquid-cooling-section](SHOTS.md#55-liquid-cooling-section), [56-power-vrm-pdn](SHOTS.md#56-power-vrm-pdn), [57-power-smoothing](SHOTS.md#57-power-smoothing)。

## BlueField-4 STX / CMX

等待、迁移和复用的KV Cache怎样进入存储层？

可用顺序：05→11→19（区分BlueField两版）→33→30/31→32→42→51。

主归属9个讲解点；交叉关联37项资产、30组镜头。

讲解点：`assembly-hierarchy`, `sram6t`, `dram1t1c`, `memory-hierarchy`, `vera-io-phy-bifurcation`, `attention-ffn`, `rdma-gpudirect`, `astra-control-data-domains`, `nand-trap-channel`, `nand-threshold-levels`, `ssd-ftl-gc`, `ssd-wear-ecc`, `kv-tensor-size`, `kv-prestage-reuse`, `nixl-memos-dynamo`, `cxl-vs-cmx`, `storage-offload`, `confidential-domains`。

镜头：[01-pod-tour](SHOTS.md#01-pod-tour), [02-rack-nvl72](SHOTS.md#02-rack-nvl72), [03-rack-vera](SHOTS.md#03-rack-vera), [04-rack-lpx](SHOTS.md#04-rack-lpx), [05-rack-stx](SHOTS.md#05-rack-stx), [06-rack-spx](SHOTS.md#06-rack-spx), [07-tray-compute](SHOTS.md#07-tray-compute), [08-tray-nvlink](SHOTS.md#08-tray-nvlink), [09-tray-vera](SHOTS.md#09-tray-vera), [10-tray-lpx](SHOTS.md#10-tray-lpx), [11-tray-stx](SHOTS.md#11-tray-stx), [12-tray-etl](SHOTS.md#12-tray-etl), [13-switch-sn6800](SHOTS.md#13-switch-sn6800), [14-switch-sn6810](SHOTS.md#14-switch-sn6810), [15-chip-vera](SHOTS.md#15-chip-vera), [18-chip-cx9](SHOTS.md#18-chip-cx9), [19-chip-bf4-dpu](SHOTS.md#19-chip-bf4-dpu), [24-pod-to-die](SHOTS.md#24-pod-to-die), [25-memory-cell-sram6t](SHOTS.md#25-memory-cell-sram6t), [26-memory-cell-dram1t1c](SHOTS.md#26-memory-cell-dram1t1c), [27-memory-cell-comparison](SHOTS.md#27-memory-cell-comparison), [29-memory-hierarchy](SHOTS.md#29-memory-hierarchy), [30-nand-charge-trap](SHOTS.md#30-nand-charge-trap), [31-nand-threshold-levels](SHOTS.md#31-nand-threshold-levels), [32-ssd-controller-ftl](SHOTS.md#32-ssd-controller-ftl), [33-kv-cache-tiers](SHOTS.md#33-kv-cache-tiers), [35-cpu-olympus-pipeline](SHOTS.md#35-cpu-olympus-pipeline), [39-prefill-decode-split](SHOTS.md#39-prefill-decode-split), [42-rdma-astra-data-path](SHOTS.md#42-rdma-astra-data-path), [51-cxl-vs-cmx](SHOTS.md#51-cxl-vs-cmx)。

## Spectrum-6 SPX / CPO

电子交换怎样连接到光纤，激光、调制、接收和封装各做什么？

可用顺序：06→12/13/14→21→43/44→45/46→23→47→48→49→50。

主归属10个讲解点；交叉关联30项资产、25组镜头。

讲解点：`assembly-hierarchy`, `packet-pipeline`, `pcs-fec`, `pam4-nrz`, `channel-equalization`, `cdr-loop`, `queue-hol-incast`, `ar-tcc-plb`, `multiplane-shuffle`, `osfp-vs-cpo`, `els-cw-modulate`, `microring-tuning`, `receive-pd-tia`, `eic-pic-package`, `laser-architecture-options`, `optical-channel-link-budget`, `mzm-vs-mrm`。

镜头：[01-pod-tour](SHOTS.md#01-pod-tour), [02-rack-nvl72](SHOTS.md#02-rack-nvl72), [03-rack-vera](SHOTS.md#03-rack-vera), [04-rack-lpx](SHOTS.md#04-rack-lpx), [05-rack-stx](SHOTS.md#05-rack-stx), [06-rack-spx](SHOTS.md#06-rack-spx), [07-tray-compute](SHOTS.md#07-tray-compute), [08-tray-nvlink](SHOTS.md#08-tray-nvlink), [09-tray-vera](SHOTS.md#09-tray-vera), [10-tray-lpx](SHOTS.md#10-tray-lpx), [11-tray-stx](SHOTS.md#11-tray-stx), [12-tray-etl](SHOTS.md#12-tray-etl), [13-switch-sn6800](SHOTS.md#13-switch-sn6800), [14-switch-sn6810](SHOTS.md#14-switch-sn6810), [21-chip-spectrum](SHOTS.md#21-chip-spectrum), [23-cpo-engine](SHOTS.md#23-cpo-engine), [24-pod-to-die](SHOTS.md#24-pod-to-die), [43-switch-packet-pipeline](SHOTS.md#43-switch-packet-pipeline), [44-network-incast-control](SHOTS.md#44-network-incast-control), [45-serdes-pam4](SHOTS.md#45-serdes-pam4), [46-serdes-equalization-cdr](SHOTS.md#46-serdes-equalization-cdr), [47-photonics-microring](SHOTS.md#47-photonics-microring), [48-photonics-laser-options](SHOTS.md#48-photonics-laser-options), [49-cpo-package-section](SHOTS.md#49-cpo-package-section), [50-network-multiplane](SHOTS.md#50-network-multiplane)。
