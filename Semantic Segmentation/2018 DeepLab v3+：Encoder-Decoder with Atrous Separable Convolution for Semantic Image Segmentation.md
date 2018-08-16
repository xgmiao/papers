













-   DeepLabv1：将空洞卷积（atrous convolution）引入语义分割任务中，避免pooling操作在扩大感受野的同时，带来信息损失的不足。同时采用CRF进行后端优化处理。
-   DeepLabv2：基于 DeepLabv1 的优化，使用空洞空间金字塔池化（atrous spatial pyramid pooling，ASPP）对物体进行有效的分割
-   DeepLabv3：采用多比例的带孔卷积级联或并行来捕获多尺度背景，基于图像特征优化，去掉了耗时的CRF。
-   ASPPDeepLabv3+ ：对 DeepLabv3 的扩展，包括一个简单而高效的改善分割结果的解码器模块 