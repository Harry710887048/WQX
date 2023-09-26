# README

### 1.使用说明

**如果您使用CPU版本，那么直接执行.exe文件即可，但运行的效率和帧率都会有所降低。**

**如果您想使用GPU版本，请按照如下步骤配置环境。请注意，可能由于路径位置存在问题，您需要根据您的本地文件路径修改文件位置。**

### 2.安装依赖

(1)为了在Windows下使用GPU加速，首先需要安装英伟达相关依赖：

- [CUDA](https://developer.nvidia.com/cuda-toolkit)
- [cuDNN](https://developer.nvidia.com/cudnn)
- [TensorRT](https://developer.nvidia.com/tensorrt)

(2)下载[ONNX Runtime](https://github.com/microsoft/onnxruntime/releases)

> 将`lib`和`include`文件夹复制到`mediapipe/calculators/tensor/onnxruntime`目录下

(3)将CUDA、cuDNN的`bin`和TensorRT的`lib`目录添加到环境变量

> 我的运行环境：
>
> - CUDA 11.7.1_516.94
> - cuDNN 8.5.0.96_cuda11
> - TensorRT 8.4.3.1
>
> 64位Windows环境下cuDNN依赖[zlib](http://www.winimage.com/zLibDll/zlib123dllx64.zip)，下载解压后将`dll_x64`目录下的`zlibwapi.dll`复制到`cuDNN`的`bin`目录下

(4)编译[Windows样例](https://github.com/liuyulvv/mediapipe/blob/main/windows_build_example.md)

如果你运行CPU版本的软件，可以不需要安装上述依赖，但效率可能会受到影响。



### 3.安装说明

在Release中下载zip文件夹，解压后，点击.exe文件，按照提示安装即可。

