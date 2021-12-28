# rust_pipeline_for_capsule

Capsule是一套供 Rust 开发者在 CKB 上开发脚本的工具，涵盖了脚本开发的整个生命周期：编写、调试、测试和部署。

这里给出部署的流程和最终结果。

* [x]  从CKB 发布页面下载最新的二进制文件。

```txt
验证  二进制文件是否正常工作并检查版本
ckb --version 
ckb-cli --version
```

![img1](./img1.png)

* [x] CKB Quick Start

run之后：

![img2](./img2.png)
ckb节点已经成功run

* [x] 添加ckb-cli到PATH环境变量中
![img3](./img3.png)

* [x] 安装docker
from https://docs.docker.com/desktop/windows/install/
等待下载，下载完成
安装...
安装遇到问题，需要wsl2 

参考 https://zhuanlan.zhihu.com/p/337104547

wsl2启用

参考
https://docs.microsoft.com/en-us/windows/wsl/install-manual#step-4---download-the-linux-kernel-update-package


hyper-v在系统设置里启用

powershell中启用
Enable-WindowsOptionalFeature -Online -FeatureName Microsoft-Hyper-V -All

这时候docker可以正常启用

powershell中输入docker run hello-world

```
Hello from Docker!
This message shows that your installation appears to be working correctly.

To generate this message, Docker took the following steps:
 1. The Docker client contacted the Docker daemon.
 2. The Docker daemon pulled the "hello-world" image from the Docker Hub.
    (amd64)
 3. The Docker daemon created a new container from that image which runs the
    executable that produces the output you are currently reading.
 4. The Docker daemon streamed that output to the Docker client, which sent it
    to your terminal.

To try something more ambitious, you can run an Ubuntu container with:
 $ docker run -it ubuntu bash

Share images, automate workflows, and more with a free Docker ID:
 https://hub.docker.com/

For more examples and ideas, visit:
 https://docs.docker.com/get-started/
```

这说明docker的安装是成功的
