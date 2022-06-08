jittor-jittor-Rush EEEEEe-计图挑战热身赛
====
 
Jittor计图挑战热身赛代码仓库。队伍：Rush EEEEEe

![主要结果](./result.png)

简介
==
  
本项目为第二届计图挑战赛热身赛的代码实现，完成了样例代码的TODO部分，成功生成了队员的手机号。

安装
==
  
运行环境
环境一
ubuntu 20.04 LTS

python >= 3.7

jittor >= 1.3.0

（可选）cuda >= 11.0

环境二
windows 10

python >= 3.8

jittor >= 1.3.0

（可选）cuda >= 11.0

安装依赖
numpy >= 1.20
预训练模型
discriminator_last.pkl与generator_last.pkl是预训练好的模型，须与CGAN.py置于同一目录下。

训练
==
  
执行python CGAN.py即可开始训练，命令行参数如下：

--n_epochs 训练epoch数，默认100
--batch_size 训练batch size，默认64
--lr adam优化器学习率，默认0.0002
--b1 adam优化器一阶动量衰减速率，默认0.5
--b2 adam优化器二阶动量衰减速率，默认0.999
--n_cpu batch生成所用cpu线程数，默认8
--latent_dim 隐空间的维数，默认100
--n_classes 数据集标签类别数目，默认10
--img_size 图片的维数，默认32
--channels 图片通道数，默认1
--sample_interval 保存图片的间隔，默认100
