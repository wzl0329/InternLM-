# Fifth_Class

![image-20240115100020118](img\img_5\image-20240115100020118.png)

![image-20240115105340979](img/img_5/image-20240115105340979.png)

![image-20240115112726409](img/img_5/image-20240115112726409.png)

![image-20240115113343570](img/img_5/image-20240115113343570.png)

![image-20240115113616781](img/img_5/image-20240115113616781.png)

![image-20240115114111262](img/img_5/image-20240115114111262.png)

![image-20240115114722487](img/img_5/image-20240115114722487.png)

![image-20240115144752790](img/img_5/image-20240115144752790.png)

![image-20240115144954565](img/img_5/image-20240115144954565.png)

![image-20240115145250296](img/img_5/image-20240115145250296.png)

![image-20240115145944800](img/img_5/image-20240115145944800.png)

![image-20240115150250523](img/img_5/image-20240115150250523.png)

![image-20240115151629332](img/img_5/image-20240115151629332.png)

 

**基础作业：**

- 使用 LMDeploy 以本地对话、网页Gradio、API服务中的一种方式部署 InternLM-Chat-7B 模型，生成 300 字的小故事（需截图）

![image-20240115184325462](img/img_5/image-20240115184325462.png)

**进阶作业（可选做）**

- 将第四节课训练自我认知小助手模型使用 LMDeploy 量化部署到 OpenXLab 平台。
- 对internlm-chat-7b模型进行量化，并同时使用KV Cache量化，使用量化后的模型完成API服务的部署，分别对比模型量化前后和 KV Cache 量化前后的显存大小（将 bs设置为 1 和 max len 设置为512）。
- 在自己的任务数据集上任取若干条进行Benchmark测试，测试方向包括：
  （1）TurboMind推理+Python代码集成
  （2）在（1）的基础上采用W4A16量化
  （3）在（1）的基础上开启KV Cache量化
  （4）在（2）的基础上开启KV Cache量化
  （5）使用Huggingface推理



进阶部分只完成了KV Cache量化和W4A16量化，

原始部署的情况下，不使用KVcache和W4A16，其显存占用为14886MB

在开启KVcache后，显存占用为14758MB，需要注意的是要将config中quant_policy改为4，只开启KVcache显存下降幅度不大。

W4A16量化显存占用仅为5984MB

W4A16量化+KVcache显存占用仅为5856MB

![image-20240116150647262](img/img_5/image-20240116150647262.png)

