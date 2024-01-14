# 计算机体系结构期末论文复现代码

中山大学    计算机学院    刘佳瑜   21311592

本存储库为MICRO22 论文《Sparseloop: 一种用于稀疏张量加速器的分析建模方法》的实验设置和关键部分复现代码，
使用Docker环境和Jupyter notebook用于评估。


### 步骤: 准备`docker-compose.yaml`
-------------------------

- 通过复制 Docker Compose 模板文件  `cp docker-compose.yaml.template docker-compose.yaml` 创建一个 Docker Compose 文件
- 查看`docker-compose.yaml` 中的说明以正确设置 Docker，即设置正确的`UID`和`GID`.


### Step 1: 获取docker
---------------------

从 Docker Hub 获取 Docker 镜像：
  ```
  docker-compose pull
  ```


### Step 2: 启动docker
--------------------
运行`docker-compose up`


### Step 3: 在 Docker 中运行实验
--------------------
导航到本项目的 workspace/2022.micro.artifact/notebook 来运行实验。
notebook中的每个单元格都提供了背景、说明和运行每个评估的命令，附带提供的脚本。

对于每个实验，给出了一个非常保守的估计，用于扫描将花费多长时间。
将生成的图表/表格与论文中的图表/表格进行比较，用以验证输出，
每个评估的详细评估结果可在ref_outputs 文件夹中查看。
