# Sixth_Class

![image-20240126143607386](img/img_6/image-20240126143607386.png)

![image-20240126143633506](img/img_6/image-20240126143633506.png)

![image-20240126143650393](img/img_6/image-20240126143650393.png)

![image-20240126160145134](img/img_6/image-20240126160145134.png)

![image-20240126160214784](img/img_6/image-20240126160214784.png)

![image-20240126164045980](img/img_6/image-20240126164045980.png)

![image-20240129173158421](img/img_6/image-20240129173158421.png)

![image-20240129173303089](img/img_6/image-20240129173303089.png)

基于prompt工程评测思路：提供相同问题的不同的prompt，看不同的prompt下，模型的表现/回答是否一致。如果随便换prompt，模型回答不对，说明模型的鲁棒性不强。

![image-20240129173629241](img/img_6/image-20240129173629241.png)

![image-20240129173733639](img/img_6/image-20240129173733639.png)

![image-20240129173751825](img/img_6/image-20240129173751825.png)

![image-20240130162059002](img/img_6/image-20240130162059002.png)

![image-20240130163031913](img/img_6/image-20240130163031913.png)



**基础作业**

- 使用 OpenCompass 评测 InternLM2-Chat-7B 模型在 C-Eval 数据集上的性能

跟着教程，# 列出所有跟 internlm 及 ceval 相关的配置

![image-20240130180954761](img/img_6/image-20240130180954761.png)

确保按照上述步骤正确安装 OpenCompass 并准备好数据集后，可以通过以下命令评测 InternLM-Chat-7B 模型在 C-Eval 数据集上的性能。由于 OpenCompass 默认并行启动评估过程，我们可以在第一次运行时以 `--debug` 模式启动评估，并检查是否存在问题。在 `--debug` 模式下，任务将按顺序执行，并实时打印输出。

![image-20240130190329996](img/img_6/image-20240130190329996.png)

![image-20240130190514429](img/img_6/image-20240130190514429.png)



**进阶作业**

- 使用 OpenCompass 评测 InternLM2-Chat-7B 模型使用 LMDeploy 0.2.0 部署后在 C-Eval 数据集上的性能

  （未完成）
