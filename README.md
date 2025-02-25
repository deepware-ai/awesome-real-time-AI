# Awesome Real-time AI ![Awesome](https://cdn.rawgit.com/sindresorhus/awesome/d7305f38d29fed78fa85652e3a63e154dd8e8829/media/badge.svg) [![Maintenance](https://img.shields.io/badge/Maintained%3F-YES-green.svg)] 

This is a list of awesome real-time AI and DNN inference related projects & papers. 

<p align="center">
  <img width="250" src="https://camo.githubusercontent.com/1131548cf666e1150ebd2a52f44776d539f06324/68747470733a2f2f63646e2e7261776769742e636f6d2f73696e647265736f726875732f617765736f6d652f6d61737465722f6d656469612f6c6f676f2e737667" "Awesome!">
</p>

## Contents
- [Benchmark and Dataset](#benchmark-and-dataset)
- [Open Source Projects](#open-source-projects)
- [Papers](#papers)
  - [Survey](#survey)
  - [DNN Compiler](#dnn-compiler)
  - [Edge-Cloud Collaborative Inference](#edge-cloud-collaborative-inference)
  - [Concurrent DNN Inference](#concurrent-dnn-inference)
  - [Heterogeneous Platforms](#heterogeneous-platforms)
  - [HPC and Archs](#hpc-and-archs)
  - [Latency Predictor](#latency-predictor)
  - [TinyML](#tinyml)
  - [Multi-modality Inference](#multi-modality-inference)
  - [Sparse Inference](#sparse-inference)
  - [Other Cool Ideas](#other-cool-ideas)
 
## Benchmark and Dataset
- [MLPerf](https://github.com/mlcommons/inference)
- [Tango: A Deep Neural Network Benchmark Suite for Various Accelerators](https://gitlab.com/Tango-DNNbench/Tango)

## Open Source Projects
- [TVM](https://tvm.apache.org/)
- [KubeEdge](https://github.com/kubeedge/kubeedge)
- [RAF](https://github.com/awslabs/raf.git)
- [INFaas](https://github.com/stanford-mast/INFaaS)
- [REEF](https://github.com/SJTU-IPADS/reef)
- [DeepSparse Engine](https://github.com/neuralmagic/deepsparse)
- [AlphaTensor](https://github.com/deepmind/alphatensor)

## Papers

### Survey
- [Edge Intelligence: Architectures, Challenges, and Applications](https://arxiv.org/pdf/2003.12172) by Xu, Dianlei, et al., arxiv 2020
- [A Survey of Multi-Tenant Deep Learning Inference on GPU](https://arxiv.org/pdf/2203.09040) by Yu, Fuxun, et al., arxiv 2022
- [Machine Learning in Real-Time Internet of Things (IoT) Systems: A Survey](https://ieeexplore.ieee.org/stamp/stamp.jsp?arnumber=9739684) by Bian, Jiang, et al., IOTJ 2022
- [AI Augmented Edge and Fog Computing: Trends and Challenges](https://arxiv.org/pdf/2208.00761) by Tuli S, Mirhakimi F, Pallewatta S, et al., arxiv 2022
- [Enable deep learning on mobile devices: Methods, systems, and applications](https://dl.acm.org/doi/pdf/10.1145/3486618) by Cai, Han, et al., TODAES 2022
- [Multi-DNN Accelerators for Next-Generation AI Systems](https://arxiv.org/pdf/2205.09376) by Venieris, Stylianos I., Christos-Savvas Bouganis, and Nicholas D. Lane., arxiv 2022
- [A Survey of GPU Multitasking Methods Supported by Hardware Architecture](https://ieeexplore.ieee.org/iel7/71/4359390/09548839.pdf) Zhao, Chen, et al., IEEE TPDS 2021

### DNN Compiler
- [TASO: The Tensor Algebra SuperOptimizer for Deep Learning](https://dl.acm.org/doi/abs/10.1145/3341301.3359630) by Zhihao Jia et al., SOSP 2019
- [AStitch: Enabling a New Multi-dimensional Optimization Space for Memory-Intensive ML Training and Inference on Modern SIMT Architectures](https://dl.acm.org/doi/10.1145/3503222.3507723) by Zhen Zheng et al., ASPLOS 2022
- [PET: Optimizing Tensor Programs with Partially Equivalent Transformations and Automated Corrections](https://www.usenix.org/conference/osdi21/presentation/wang) by Haojie Wang et al., OSDI 2021
- [Rammer: Enabling Holistic Deep Learning Compiler Optimizations with rTasks](https://www.usenix.org/conference/osdi20/presentation/ma) by Lingxiao Ma et al., OSDI 2020
- [TASO: The Tensor Algebra SuperOptimizer for Deep Learning](https://dl.acm.org/doi/abs/10.1145/3341301.3359630) by Zhihao Jia et al., SOSP 2019
- [Bolt: Bridging the Gap between Auto-tuners and Hardware-native Performance](https://proceedings.mlsys.org/paper/2022/hash/38b3eff8baf56627478ec76a704e9b52-Abstract.html) by Jiarong Xing et al., MLSys 2022
- [Ansor: Generating High-Performance Tensor Programs for Deep Learning](https://arxiv.org/abs/2006.06762) by Lianmin Zheng et al., OSDI 2020
- [TenSet: A Large-scale Program Performance Dataset for Learned Tensor Compilers](https://datasets-benchmarks-proceedings.neurips.cc/paper/2021/hash/a684eceee76fc522773286a895bc8436-Abstract-round1.html) by Lianmin Zheng., NeurIPS 2021
- [Romou: Rapidly Generate High-Performance Tensor Kernels for Mobile GPUs](https://www.microsoft.com/en-us/research/uploads/prod/2022/02/mobigpu_mobicom22_camera.pdf) by Liang, Rendong, et al., MobiCom 2022
- [Asymo: scalable and efficient deep-learning inference on asymmetric mobile cpus](https://dl.acm.org/doi/abs/10.1145/3447993.3448625) by Wang, Manni, et al., MobiCom 2021
- [Ios: Inter-operator scheduler for cnn acceleration](https://proceedings.mlsys.org/paper/2021/file/38b3eff8baf56627478ec76a704e9b52-Paper.pdf) by Ding, Yaoyao, et al., MLSys 2021
- [Moses: Efficient Exploitation of Cross-device Transferable Features for Tensor Program Optimization](https://arxiv.org/pdf/2201.05752) by Zhao, Zhihe, et al., arxiv 2022
- [DeepCuts: A Deep Learning Optimization Framework for Versatile GPU Workloads](https://dl.acm.org/doi/pdf/10.1145/3453483.3454038) by Jung, Wookeun, Thanh Tuan Dao, and Jaejin Lee., PLDI 2021
- [CASE: a compiler-assisted SchEduling framework for multi-GPU systems](https://dl.acm.org/doi/pdf/10.1145/3503221.3508423?casa_token=c738_W6lYCkAAAAA:QcpPBlGQcRjbfbnr99-N7fJXV5ssZMVL9odTdrfRFRLXtaOcAAQOeh3JwhEeaQvOEpX1IRJquURmTg) by Chen, Chao, Chris Porter, and Santosh Pande., PPoPP 2022
- [Chameleon: Adaptive code optimization for expedited deep neural network compilation](https://arxiv.org/pdf/2001.08743) by Ahn, Byung Hoon, et al., arxiv 2020
- [Analytical characterization and design space exploration for optimization of CNNs](https://dl.acm.org/doi/pdf/10.1145/3445814.3446759) by Li, Rui, et al., ASPLOS 2021
- [DNNFusion: accelerating deep neural networks execution with advanced operator fusion](https://dl.acm.org/doi/pdf/10.1145/3453483.3454083) by Niu, Wei, et al., PLDI 2021
- [AutoGTCO: Graph and Tensor Co-Optimize for Image Recognition with Transformers on GPU](https://ieeexplore.ieee.org/iel7/9643423/9643432/09643487.pdf?casa_token=LyByXa84XpMAAAAA:4qRC6_8TE6iVgSlL0NMKy4tRJ6aoDB47fqcGVxhwM7dL1nddqsVuIs2dAmHVGrCN8dBhTCE) by Bai, Yang, et al., ICCAD 2021
- [DietCode: Automatic Optimization for Dynamic Tensor Programs](https://proceedings.mlsys.org/paper/2022/file/fa7cdfad1a5aaf8370ebeda47a1ff1c3-Paper.pdf) by Zheng, Bojian, et al., MLSys 2022
- [ROLLER: Fast and Efficient Tensor Compilation for Deep Learning](https://www.usenix.org/system/files/osdi22-zhu.pdf) by Zhu, Hongyu, et al., OSDI 2022
- [FamilySeer: Towards Optimized Tensor Codes by Exploiting Computation Subgraph Similarity](https://arxiv.org/pdf/2201.00194) by Zhang, Shanjun, et al., arxiv 2022
- [Reusing Auto-Schedules for Efficient DNN Compilation](https://arxiv.org/pdf/2201.05587) by Gibson, Perry, and José Cano., arxiv 2022
- [Hidet: Task Mapping Programming Paradigm for Deep Learning Tensor Programs](https://scholar.google.com/scholar?hl=en&as_sdt=0%2C5&q=Hidet%3A+Task+Mapping+Programming+Paradigm+for+Deep+Learning+Tensor+Programs&btnG=#d=gs_cit&t=1666445708655&u=%2Fscholar%3Fq%3Dinfo%3Ahj_cZ1YLpt8J%3Ascholar.google.com%2F%26output%3Dcite%26scirp%3D0%26hl%3Den) by Ding, Yaoyao, et al., arxiv 2022

### Edge-Cloud Collaborative Inference
- [EdgeML: An AutoML framework for real-time deep learning on the edge](https://dl.acm.org/doi/10.1145/3450268.3453520) by Zhao, Zhihe, et al., IoTDI 2021
- [SPINN: synergistic progressive inference of neural networks over device and cloud](https://dl.acm.org/doi/pdf/10.1145/3372224.3419194) by Laskaridis, Stefanos, et al., MobiCom 2020
- [Clio: Enabling automatic compilation of deep learning pipelines across iot and cloud](https://dl.acm.org/doi/pdf/10.1145/3372224.3419215?casa_token=XuIaaSOhXj8AAAAA:yC9swMPqSUSKBfe8yFelcaUvzBb3VHrpYroB87OFI0XgbEDZ6-EQipQFpnP9aduYdB3kjOu0MdNcRg) by Huang, Jin, et al., MobiCom 2020
- [Neurosurgeon: Collaborative intelligence between the cloud and mobile edge](https://dl.acm.org/doi/pdf/10.1145/3093337.3037698) by Kang, Yiping, et al., ASPLOS 2017
- [Mistify: Automating DNN Model Porting for On-Device Inference at the Edge](https://www.usenix.org/system/files/nsdi21-guo.pdf) by Guo, Peizhen et al., NSDI 2021
- [Deep compressive offloading: Speeding up neural network inference by trading edge computation for network latency.](https://dl.acm.org/doi/pdf/10.1145/3384419.3430898) by Yao, Shuochao, et al., SenSys 2020
- [Elf: accelerate high-resolution mobile deep vision with content-aware parallel offloading](https://dl.acm.org/doi/pdf/10.1145/3447993.3448628) by Zhang, Wuyang, et al., MobiCom 2021
- [Edge assisted real-time object detection for mobile augmented reality](https://dl.acm.org/doi/pdf/10.1145/3300061.3300116) by Liu, Luyang, Hongyu Li, and Marco Gruteser., MobiCom 2019

### Concurrent DNN Inference
- [VELTAIR: towards high-performance multi-tenant deep learning services via adaptive compilation and scheduling](https://dl.acm.org/doi/pdf/10.1145/3503222.3507752?casa_token=4WEkiHRYJHEAAAAA:Ae8yvTck-swW5LDJ3Cx3spak5Q2IzfRIVvPAvEG3zHkCudGBF0R4-XxeJk1hBaS4LmzCmxaAqNenCg) by Liu, Zihan, et al., ASPLOS 2021
- [RT-mDL: Supporting Real-Time Mixed Deep Learning Tasks on Edge Platforms](https://dl.acm.org/doi/pdf/10.1145/3485730.3485938?casa_token=gmqsW0h-7TUAAAAA:MqWvebvOkaT0kCORWXPCoIN5VEN0EBToR36zucKe63d1Exf9m-a5H8ebHVO2-OZZh6YB7DzvytW8QQ) by Ling, Neiwen, et al., SenSys 2021
- [Horus: Interference-aware and prediction-based scheduling in deep learning systems](https://ieeexplore.ieee.org/iel7/71/4359390/09428512.pdf) by Yeung, Gingfung, et al., IEEE TPDS 2021
- [Automated Runtime-Aware Scheduling for Multi-Tenant DNN Inference on GPU](https://ieeexplore.ieee.org/iel7/9643423/9643432/09643501.pdf) by Yu, Fuxun, et al., ICCAD 2021
- [Interference-aware scheduling for inference serving](https://dl.acm.org/doi/pdf/10.1145/3437984.3458837?casa_token=CWMAG53X-EoAAAAA:FXA3ZHvAzasGqkaUPoVoXNREe1qEzYkaFQramYjfG_mu0MjJVJdQzH_IjBPGAIuhkmq9CgPuAQ) by Mendoza, Daniel, et al., EuroMLSys 2021
- [Microsecond-scale Preemption for Concurrent GPU-accelerated DNN Inferences](https://www.usenix.org/system/files/osdi22-han.pdf) by Han, Mingcong, et al., OSDI 2022
- [Planaria: Dynamic architecture fission for spatial multi-tenant acceleration of deep neural networks](https://ieeexplore.ieee.org/iel7/9251289/9251849/09251939.pdf?casa_token=JK4fOIekLU0AAAAA:zLGfIHmDMqPICBSEjAYEa1xHuFRBXTN4Kc-bjO8eZD-VhVIuNlV2B_UCCSXdFY-bWUSOC1xbJqM) by Ghodrati, Soroush, et al., MICRO 2020
- [Heimdall: mobile GPU coordination platform for augmented reality applications](https://dl.acm.org/doi/pdf/10.1145/3372224.3419192?casa_token=TDdZgOLYfioAAAAA:w_HWQIpOiic498lYa-z6kRUYp4RxS92RiVoxNP6P6vBR7QvK2wyAYS4h77wEIh9ogv6B1n29zwfedw) by Yi, Juheon, and Youngki Lee., MobiCom 2020
- [Deepeye: Resource efficient local execution of multiple deep vision models using wearable commodity hardware](https://dl.acm.org/doi/pdf/10.1145/3081333.3081359) by Mathur, Akhil, et al., MobiSys 2017
- [PipeSwitch: Fast Pipelined Context Switching for Deep Learning Applications](https://www.usenix.org/system/files/osdi20-bai.pdf) by Bai, Zhihao, et al., OSDI 2020
- [Enable simultaneous DNN services based on deterministic operator overlap and precise latency prediction](https://dl.acm.org/doi/pdf/10.1145/3458817.3476143) by Cui, Weihao, et al., SC 2021
- [LegoDNN: block-grained scaling of deep neural networks for mobile vision](https://dl.acm.org/doi/abs/10.1145/3447993.3483249) by Han, Rui, et al., MobiCom 2021
- [NeuOS: A Latency-Predictable Multi-Dimensional Optimization Framework for DNN-driven Autonomous Systems](https://www.usenix.org/system/files/atc20-bateni.pdf) by Bateni, Soroush, and Cong Liu., ATC 2020
- [Multi-Neural Network Acceleration Architecture](https://ieeexplore.ieee.org/iel7/9136582/9138908/09138929.pdf) by Baek, Eunjin, Dongup Kwon, and Jangwoo Kim., ISCA 2020
- [Pipelined data-parallel CPU/GPU scheduling for multi-DNN real-time inference](https://ieeexplore.ieee.org/iel7/9040680/9052112/09052147.pdf) by Xiang, Yecheng, and Hyoseung Kim., RTSS 2019
- [Nestdnn: Resource-aware multi-tenant on-device deep learning for continuous mobile vision](https://dl.acm.org/doi/pdf/10.1145/3241539.3241559) by Fang, Biyi, Xiao Zeng, and Mi Zhang., MobiCom 2018
- [Flep: Enabling flexible and efficient preemption on gpus](https://dl.acm.org/doi/pdf/10.1145/3093336.3037742) by Wu, Bo, et al., ASPLOS 2017
- [Prophet: Precise qos prediction on non-preemptive accelerators to improve utilization in warehouse-scale computers](https://dl.acm.org/doi/pdf/10.1145/3037697.3037700) by Chen, Quan, et al., ASPLOS 2017
- [PAME: precision-aware multi-exit DNN serving for reducing latencies of batched inferences](https://dl.acm.org/doi/pdf/10.1145/3524059.3532366?casa_token=D31LanqCaE4AAAAA:BSK0aEULjkZAYdi0H6Xionzf1MkbCSxVoKlZJNKkGbpTdGf2iJ3mBxBGmERIU4toYqSlVcDKyA) by Zhang, Shulai, et al., ICS 2022
- [Layerweaver: Maximizing resource utilization of neural processing units via layer-wise scheduling](https://ieeexplore.ieee.org/iel7/9406784/9407034/09407236.pdf) by Oh, Young H., et al., HPCA 2021
- [LiteReconfig: cost and content aware reconfiguration of video object detection systems for mobile GPUs](https://dl.acm.org/doi/pdf/10.1145/3492321.3519577) by Xu, Ran, et al., EuroSys 2022
- [ApproxNet: Content and contention-aware video object classification system for embedded clients](https://dl.acm.org/doi/pdf/10.1145/3463530) Xu, Ran, et al. 

### Heterogeneous Platforms
- [Lalarand: Flexible layer-by-layer cpu/gpu scheduling for real-time dnn tasks](https://ieeexplore.ieee.org/iel7/9622323/9622324/09622325.pdf?casa_token=HtllgvtNt8wAAAAA:hasDDmtMmf8uVWgtrevp1XT2Ldh4u-0bWMjup4VPqT1PsCbq77cgwOMOAeAboXs_J_Goklo) by Kang, Woosung, et al., RTSS 2021
- [DUET: A Compiler-Runtime Subgraph Scheduling Approach for Tensor Programs on a Coupled CPU-GPU Architecture](https://dl.acm.org/doi/pdf/10.1145/3442442.3452297?casa_token=rNEtNHavbREAAAAA:U4wL45EN3WD8dh_CW41BVZSAcdKCzDO1KRvNRJsCIMTk6SoeaUa2NvvosOkN6vLnCLcZHt7sMg) by Zhang, Minjia, Zehua Hu, and Mingqin Li., IPDPS 2021
- [Band: coordinated multi-DNN inference on heterogeneous mobile processors](https://dl.acm.org/doi/pdf/10.1145/3498361.3538948) by Jeong, Joo Seong, et al., MobiSys 2022
- [ODMDEF: On-Device Multi-DNN Execution Framework Utilizing Adaptive Layer-Allocation on General Purpose Cores and Accelerator](https://ieeexplore.ieee.org/iel7/6287639/9312710/09453793.pdf) by Lim, Cheolsun, and Myungsun Kim., IEEE ACCESS 2021
- [μlayer: Low latency on-device inference using cooperative single-layer acceleration and processor-friendly quantization](https://dl.acm.org/doi/pdf/10.1145/3302424.3303950) by Kim, Youngsok, et al., EuroSys 2019
- [OPTiC: Optimizing collaborative CPU–GPU computing on mobile devices with thermal constraints](https://ieeexplore.ieee.org/iel7/43/6917053/08477038.pdf) by Wang, Siqi, Gayathri Ananthanarayanan, and Tulika Mitra., TCAD 2019
- [Accelerating Sequence-to-Graph Alignment on Heterogeneous Processors](https://dl.acm.org/doi/pdf/10.1145/3472456.3472505) by Feng, Zonghao, and Qiong Luo., ICPP 2021
- [Efficient Execution of Deep Neural Networks on Mobile Devices with NPU](https://dl.acm.org/doi/pdf/10.1145/3412382.3458272) by Tan, Tianxiang, and Guohong Cao., IPSN 2021
- [CoDL: efficient CPU-GPU co-execution for deep learning inference on mobile devices](https://www.microsoft.com/en-us/research/uploads/prod/2022/05/mobisys22-CoDL__Efficient_CPU_GPU_Co_execution_for_DL_Model_Inference_on_Mobile_Devices-4.pdf) by Jia, Fucheng, et al., MobiSys 2022
- [Coda: Improving resource utilization by slimming and co-locating dnn and cpu jobs](https://ieeexplore.ieee.org/iel7/9355572/9355578/09355823.pdf) by Zhao, Han, et al. ICDCS 2020


### HPC and Archs
- [GPUReplay: a 50-KB GPU stack for client ML](https://dl.acm.org/doi/pdf/10.1145/3503222.3507754) by Park, Heejin, and Felix Xiaozhu Lin., ASPLOS 2022
- [Real-time high performance computing using a Jetson Xavier AGX](https://hal.archives-ouvertes.fr/hal-03693764/document) by Cetre, Cyril, et al., ERTS 2022
- [GPU scheduling on the NVIDIA TX2: Hidden details revealed](https://ieeexplore.ieee.org/iel7/8272883/8277266/08277284.pdf) by Amert, Tanya, et al., RTSS 2017
- [Nimble: Lightweight and parallel gpu task scheduling for deep learning](https://proceedings.neurips.cc/paper/2020/file/5f0ad4db43d8723d18169b2e4817a160-Paper.pdf) by Kwon, Woosuk, et al., NeurIPS 2020
- [Addressing GPU on-chip shared memory bank conflicts using elastic pipeline](https://link.springer.com/content/pdf/10.1007/s10766-012-0201-1.pdf) by Gou, Chunyang, and Georgi N. Gaydadjiev., IJPP 2013
- [A study of persistent threads style GPU programming for GPGPU workloads](https://ieeexplore.ieee.org/iel5/6330715/6339585/06339596.pdf) by Gupta, Kshitij, Jeff A. Stuart, and John D. Owens., IEEE 2012
- [Demystifying the placement policies of the NVIDIA GPU thread block scheduler for concurrent kernels](https://dl.acm.org/doi/pdf/10.1145/3453953.3453972) by Gilman, Guin, et al., ACM SIGMETRICS Performance Evaluation Review 2021 
- [Exploiting Intra-SM Parallelism in GPUs via Persistent and Elastic Blocks](https://ieeexplore.ieee.org/iel7/9643591/9643617/09643686.pdf) by Zhao, Han, et al., ICDC 2021
- [Online Thread Auto-Tuning for Performance Improvement and Resource Saving](https://ieeexplore.ieee.org/iel7/71/4359390/09762963.pdf) by Luan, Guangqiang, et al., IEEE TPDS 2021
- [Hsm: A hybrid slowdown model for multitasking gpus](https://dl.acm.org/doi/pdf/10.1145/3373376.3378457) by Zhao, Xia, Magnus Jahre, and Lieven Eeckhout., ASPLOS 2020
- [Enabling and exploiting flexible task assignment on GPU through SM-centric program transformations](https://dl.acm.org/doi/pdf/10.1145/2751205.2751213) by Wu, Bo, et al., ACM ICS 2015
- [Warped-Slicer: Efficient Intra-SM Slicing through Dynamic Resource Partitioning for GPU Multiprogramming](https://ieeexplore.ieee.org/iel7/7551325/7551326/07551396.pdf) by Xu, Qiumin, et al., ISCA 2016
- [Kernelet: High-Throughput GPU Kernel Executions with Dynamic Slicing and Scheduling](https://ieeexplore.ieee.org/iel7/71/4359390/06624111.pdf) by Zhong, Jianlong, and Bingsheng He. IEEE TPDS 2013
- [Improving GPGPU concurrency with elastic kernels](https://dl.acm.org/doi/pdf/10.1145/2490301.2451160) by Pai, Sreepathi, Matthew J. Thazhuthaveetil, and Ramaswamy Govindarajan., ACM SIGARCH Computer Architecture News 2013
- [Neither More Nor Less: Optimizing Thread-level Parallelism for GPGPUs](https://ieeexplore.ieee.org/iel7/6603429/6618788/06618813.pdf) Kayıran, Onur, et al. ICPCT 2013
- [Orion: A framework for gpu occupancy tuning](https://dl.acm.org/doi/pdf/10.1145/2988336.2988355) by Hayes, Ari B., et al., International Middleware Conference. 2016
- [Efficient performance estimation and work-group size pruning for OpenCl kernels on GPUs](https://ieeexplore.ieee.org/iel7/71/4359390/08928962.pdf) by Wang, Xiebing, et al., IEEE TPDS 2019
- [Online evolutionary batch size orchestration for scheduling deep learning workloads in GPU clusters](https://dl.acm.org/doi/pdf/10.1145/3458817.3480859) by Bian, Zhengda, et al., SC 2021
- [Autotuning GPU kernels via static and predictive analysis](https://ieeexplore.ieee.org/iel7/8023017/8025263/08025326.pdf) by Lim, Robert, Boyana Norris, and Allen Malony., IEEE ICPP 2017
- [Gslice: controlled spatial sharing of gpus for a scalable inference platform](https://dl.acm.org/doi/pdf/10.1145/3419111.3421284) by Dhakal, Aditya, Sameer G. Kulkarni, and K. K. Ramakrishnan., SOCC 2020

### Latency Predictor
- [MAPLE-X: Latency Prediction with Explicit Microprocessor Prior Knowledge](https://arxiv.org/pdf/2205.12660) by Abbasi, Saad, Alexander Wong, and Mohammad Javad Shafiee., arxiv 2022
- [MAPLE-Edge: A Runtime Latency Predictor for Edge Devices](https://openaccess.thecvf.com/content/CVPR2022W/EVW/papers/Nair_MAPLE-Edge_A_Runtime_Latency_Predictor_for_Edge_Devices_CVPRW_2022_paper.pdf) by Nair, Saeejith, et al., CVPR 2022
- [Maple: Microprocessor a priori for latency estimation](https://openaccess.thecvf.com/content/CVPR2022W/ECV/papers/Abbasi_MAPLE_Microprocessor_a_Priori_for_Latency_Estimation_CVPRW_2022_paper.pdf) by Abbasi, Saad, Alexander Wong, and Mohammad Javad Shafiee., CVPR 2022
- [nn-Meter: towards accurate latency prediction of deep-learning model inference on diverse edge devices](https://dl.acm.org/doi/pdf/10.1145/3458864.3467882?casa_token=XqdJMALxIdkAAAAA:VhfaRoo7fWSlLOERqfqPcTjW4NfsBB0EXG7AKTw-s_eUFjMscdzTK6oU1kAPREY6nlF2jqO43PTk6g) by Zhang, Li Lyna, et al., MobiSys 2021
- [Wei, Mengze, et al. "Predicting and reining in application-level slowdown on spatial multitasking GPUs.](https://www.sciencedirect.com/science/article/pii/S0743731519307361) by Wei, Mengze, et al., JPDC 2020


### TinyML
- [Mcunet: Tiny deep learning on iot devices](https://proceedings.neurips.cc/paper/2020/file/86c51678350f656dcc7f490a43946ee5-Paper.pdf) by Lin, Ji, et al. , NeurIPS 2020
- [TinyML: Current Progress, Research Challenges, and Future Roadmap](https://ieeexplore.ieee.org/iel7/9585997/9586083/09586232.pdf?casa_token=OkZ2VanNSfoAAAAA:VepU071luwbGdzcLFA_4bHRlLXZ-CRo2Xwsw-7kLKF8BBLw_2eI83V52l8kc8XP93MwUwHxArgI) by Shafique, Muhammad, et al., DAC 2021
- [Benchmarking TinyML systems: Challenges and direction](https://arxiv.org/pdf/2003.04821) by Banbury, Colby R., et al., arxiv 2020
- [μNAS: Constrained Neural Architecture Search for Microcontrollers](https://dl.acm.org/doi/pdf/10.1145/3437984.3458836) by Liberis, Edgar, Łukasz Dudziak, and Nicholas D. Lane., EuroMLSys 2021
- [Memory-efficient Patch-based Inference for Tiny Deep Learning](https://proceedings.neurips.cc/paper/2021/file/1371bccec2447b5aa6d96d2a540fb401-Paper.pdf) by Lin, Ji, et al., NeurIPS 2021
- [Deep Learning on Microcontrollers: A Study on Deployment Costs and Challenge](https://dl.acm.org/doi/pdf/10.1145/3517207.3526978) by Filip Svoboda, Javier Fernandez-Marques, Edgar Liberis, Nicholas D Lane, EuroMLSys 2022

### Multi-modality Inference
- [Dynamic Multimodal Fusion](https://arxiv.org/abs/2204.00102) by Xue, Zihui, and Radu Marculescu., arxiv 2022
- [LM-Nav: Robotic Navigation with Large Pre-Trained Models of Language, Vision, and Action](https://arxiv.org/pdf/2207.04429) by Shah, Dhruv, et al., arxiv 2022
- [Accelerating mobile audio sensing algorithms through on-chip gpu offloading](https://dl.acm.org/doi/pdf/10.1145/3081333.3081358) by Georgiev, Petko, et al., MobiSys 2017

### Sparse Inference
- [SparTA: Deep-Learning Model Sparsity via Tensor-with-Sparsity-Attribute](https://www.usenix.org/system/files/osdi22-zheng-ningxin.pdf) by Zheng, Ningxin, et al., OSDI 2022
- [ESCALATE: Boosting the Efficiency of Sparse CNN Accelerator with Kernel Decomposition](https://dl.acm.org/doi/pdf/10.1145/3466752.3480043) by Li, Shiyu, et al., MICRO 2021
- [A high-performance sparse tensor algebra compiler in Multi-Level IR](https://arxiv.org/pdf/2102.05187) by Tian, Ruiqin, et al., arxiv 2021
- [Efficient Sparse Matrix Kernels based on Adaptive Workload-Balancing and Parallel-Reduction](https://arxiv.org/pdf/2106.16064) by Huang, Guyue, et al., arxiv 2021
- [COEXE: An Efficient Co-execution Architecture for Real-Time Neural Network Services](https://ieeexplore.ieee.org/iel7/9211868/9218488/09218740.pdf) by Liu, Chubo, et al., DAC 2020
- [TorchSparse: Efficient Point Cloud Inference Engine](https://proceedings.mlsys.org/paper/2022/file/6512bd43d9caa6e02c990b0a82652dca-Paper.pdf) by Tang, Haotian, et al., MLSys 2022

### Other Cool Ideas
- [Understanding and Optimizing Deep Learning Cold-Start Latency on Edge Devices](https://arxiv.org/pdf/2206.07446) by Yi, Rongjie, et al., arxiv 2022
- [Towards efficient vision transformer inference: a first study of transformers on mobile devices](https://dl.acm.org/doi/pdf/10.1145/3508396.3512869) by Wang, Xudong, et al., HotMobile 2022
- [Edgebert: Sentence-level energy optimizations for latency-aware multi-task nlp inference](https://dl.acm.org/doi/pdf/10.1145/3466752.3480095) by Tambe, Thierry, et al., MICRO 2021
- [EDGEWISE: A Better Stream Processing Engine for the Edge](https://www.usenix.org/system/files/atc19-fu.pdf) by Fu, Xinwei, et al., ATC 2019
- [LiteFlow: towards high-performance adaptive neural networks for kernel datapath](https://cse.hkust.edu.hk/~kaichen/papers/liteflow-sigcomm22.pdf) by Zhang, Junxue, et al., SIGCOMM 2022
- [CoCoPIE: Making Mobile AI Sweet As PIE--Compression-Compilation Co-Design Goes a Long Way](https://arxiv.org/pdf/2003.06700) by Liu, Shaoshan, et al., arxiv 2020
- [Beyond Data and Model Parallelism for Deep Neural Networks](https://proceedings.mlsys.org/paper/2019/file/c74d97b01eae257e44aa9d5bade97baf-Paper.pdf) by Jia, Zhihao, Matei Zaharia, and Alex Aiken, MLSys 2019
- [Discovering faster matrix multiplication algorithms with reinforcement learning](https://www.nature.com/articles/s41586-022-05172-4) by Fawzi, Alhussein, et al., Nature 2022


