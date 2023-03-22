<div align="center">
  <img src="https://github.com/LumosNet/Lumos/blob/master/img/Lumos.png">
</div>

# Lumos Build
## 简介

[Lumos](https://gitee.com/lumos-net/lumos)框架的发行版本存放仓库，您可以在这里找到所有lumos框架的历史版本

## 历史版本

版本                    | 链接                                                                                                                                                                           | Coretype
----------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------
**v0.1**                 | [<img src="https://img.shields.io/badge/Lumos-CPU-brightgreen" />](https://github.com/LumosNet/Lumos-Build/raw/main/v0.1.0/lumos_0.1.0_linux_cpu.run)           | CPU
**v0.1**                 | [<img src="https://img.shields.io/badge/Lumos-GPU-brightgreen" />](https://github.com/LumosNet/Lumos-Build/raw/main/v0.1.0/lumos_0.1.0_linux_gpu.run)           | GPU

## 安装

### **Linux**

使用如下命令进行安装

```shell
$ sudo sh lumos_0.1.0_linux_cpu.run
```

添加环境变量，在用户目录下~/.bashrc文件末尾添加如下语句

```
export PATH=/usr/local/lumos/bin${PATH:+:${PATH}}
export LD_LIBRARY_PATH=/usr/local/lumos/lib${LD_LIBRARY_PATH:+:${LD_LIBRARY_PATH}}
```

添加完成后，在命令行运行

```shell
source ~/.bashrc
```

来激活相关设置，此时您已经完成lumos的安装

通过命令行验证安装

```shell
lumos --version
```

若出现以下版本信息，则您已经安装好了lumos

```shell
Lumos version: v0.1
This is free software; see the source for copying conditions.  There is NO
warranty; not even for MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.
```

### **Cuda**

Lumos支持cuda加速，如果您拥有支持cuda的GPU，并且希望使用GPU加速您的算法，那么请提前安装cuda，相关安装方法请参考[cuda文档](https://docs.nvidia.com/cuda/cuda-toolkit-release-notes/index.html)

