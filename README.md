# License_Plate_Recognition
车牌识别
车牌检测模块使用retinaface，原始的retinaface是做人脸检测的，它能输出人脸检测矩形框和人脸5个关键点。考虑到车牌只有4个点，于是修改retinaface的网络结构使其输出4个关键点，然后在车牌数据集训练，训练完成后，以一幅图片上做目标检测的结果如上图所示。车牌矫正模块使用了传统图像处理方法，关键函数是opencv里的getPerspectiveTransform和warpPerspective。车牌识别模块使用Intel公司提出的LPRNet
