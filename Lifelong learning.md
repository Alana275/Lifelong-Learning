
# Lifelong learning 

## What's Lifelong learning/Continuous Learning?

终身学习（Lifelong Learning，LL）是一个持续学习的过程。在任一时间点，学习器已经执行了N个学习任务T1,T2,…,TN，这些任务也被称为先前任务（previous task），并且有各自对应的数据集D1,D2,…,DN。这些任务可以是不同类型（type），也可属于不同领域（domain）。当遇到第N+1个任务TN+1（被称为新任务或者当前任务）和其对应的数据集DN+1时，学习器可以利用知识库中的历史知识来帮助学习TN+1。这个任务可以是给定的，也可以是系统自身检测出来的（这将在后面进行介绍）。终身学习的目标通常是优化新任务TN+1的性能，但是它可以通过将其余任务视为先前任务来优化任何任务。知识库维护先前学习到的知识，并通过学习先前任务来进行知识积累。当完成学习TN+1后，根据从TN+1中学习到的知识（例如，中间和最后的结果）对知识库进行更新。这种更新包括更高层次知识的一致性检查、推理和元挖掘。

理想的情况下，一个终身学习器应该具有以下功能：
在开放环境下学习和运作，不仅可以运用学到的模型和知识来解决问题，而且还能发现要学习的新任务。
在应用和测试已学模型的过程中学会优化模型性能。这就像是职业培训之后，我们应会边做边学来提升工作技能。

在目前的研究中，终身学习算法的实验性评估通常遵循以下步骤：

1. 在先前任务的数据上运行：首先在一组先前任务的数据上运行算法，按指定的顺序每次运行一个，并将获得的知识保存到知识库。用来做实验的算法可以有多种变体或版本（例如，使用不同类型的知识，以及或多或少的知识）。

2. 在新任务的数据上运行：接下来利用知识库中的知识在新任务的数据上运行终身学习算法。

3. 运行基准算法：为了进行比较，运行一些基准算法。通常有两种类型的基准算法：第一种是在不使用任何过去知识的情况下对新数据执行孤立学习的算法，第二种是现有的终身学习算法。

4. 分析结果：比较步骤2和3的结果并加以分析、观察，以证明步骤2中终身学习算法的结果要优于步骤3中基准算法的结果。

From *Lifelong Machine Learning, Second Edition*


## Papers

### CV(Computer Vision)

- RECALL: Replay-based Continual Learning in Semantic Segmentation.
  [[pdf]](https://arxiv.org/abs/2108.03673.pdf)
  [[code]](https://github.com/lttm/recall)
  - Andrea Maracani, Umberto Michieli, Marco Toldo, Pietro Zanuttigh. *ICCV 2021*

- Few-Shot and Continual Learning with Attentive Independent Mechanisms.
  [[pdf]](hhttps://arxiv.org/abs/2107.14053.pdf)
  [[code]](https://github.com/huang50213/AIM-Fewshot-Continual)
  - Eugene Lee, Cheng-Han Huang, Chen-Yi Lee. *ICCV 2021*

### Knowledge Distillation and Incremental Learning

- Hyper-LifelongGAN: Scalable Lifelong Learning for Image Conditioned Generation.
  [[pdf]](https://openaccess.thecvf.com/content/CVPR2021/papers/Zhai_Hyper-LifelongGAN_Scalable_Lifelong_Learning_for_Image_Conditioned_Generation_CVPR_2021_paper.pdf)
  - Mengyao Zhai, Lei Chen, Greg Mori. *CVPR 2021*

- Efficient Feature Transformations for Discriminative and Generative Continual Learning.
  [[pdf]](https://arxiv.org/abs/2103.13558)
  - Vinay Kumar Verma, Kevin J Liang, Nikhil Mehta, Piyush Rai, Lawrence Carin. *CVPR 2021*
 
- Learning From Temporal Gradient for Semi-Supervised Action Recognition.
  [[pdf]](https://arxiv.org/abs/2111.13241)
  - Junfei Xiao, Longlong Jing, Lin Zhang, Ju He, Qi She, Zongwei Zhou, Alan Yuille, Yingwei Li. *CVPR 2022*

- Dark Experience for General Continual Learning: a Strong, Simple Baseline.
  [[pdf]](https://arxiv.org/pdf/2004.07211.pdf)
  [[code]](https://github.com/aimagelab/mammoth)
  - Pietro Buzzega, Matteo Boschini, Angelo Porrello, Davide Abati, Simone Calderara. *NeurIPS 2020*



## Reference
[1] https://github.com/TouchSky-Lab/Awesome-Lifelong-Continual-Learning