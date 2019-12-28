# 自然语言生成(NLG)
#### **什么是自然语言生成(NLG)?**<br>
&ensp;&ensp;&ensp;&ensp;自然语言生成(NLG)是一种语言技术，其主要目的是构建能够“写”的软件系统的技术，即能够用汉语、英语等其他人类语言生成解释、摘要、叙述等。具体来说就是计算机的“编写语言”，它将结构化数据转换为文本，以人类语言表达。即能够根据一些关键信息及其在机器内部的表达形式，经过一个规划过程，来自动生成一段高质量的自然语言文本。NLG用于Email、手机短信，它可以为您自动创建答复；NLG用于图标说明时，可以根据公司数据自动生成图标说明。前段时间在一个有趣的用例中，美联社利用自然语言生成成功的从公司收益报表中生成了报告。这意味着他们不再需要人类消耗他们的时间和精力去解决这些问题。更重要的是，NLG一旦被完美设置就会自动生成数以千计的报告。<br>

#### **学术研究介绍**<br>
&ensp;&ensp;&ensp;&ensp;NLG学术界每年都会召开会议，公布NLG的最新发现。这些会议是由[ACL SIGGEN](https://aclweb.org/aclwiki/SIGGEN)组织的，你可以查看其web页面以获取关于即将举行的活动的信息。在这些活动中提交的论文可以通过[ACL Anthology](https://www.aclweb.org/anthology/)在线获得。NLG的商业兴趣日益增长，其中大部分集中在数据到文本，即结合NLG和数据分析的系统，以产生摘要，解释等结构化数据.<br>
    
## 资料分享
### 国内外知名大佬博客
#### **Ehud Reiter** 
&ensp;&ensp;&ensp;&ensp;Ehud Reiter是阿伯丁大学的计算机科学教授，同时也是Arria NLG的首席科学家，主要专注于自然语言生成(NLG)技术，即利用人工智能和自然语言处理技术，将非语言数据自动生成高质量文本和叙述文章。他的博客[Ehud Reiter's Blog](https://ehudreiter.com/blog-index/)主要包括：NLG系统的搭建、NLG系统性能的评估、NLG的学术生活、NLG相关话题、个人生活等五个部分，该博客对NLG技术、评价与应用进行了深入的探讨与反思。其中有一篇文章我觉得写得特别不错‘How do I Learn about NLG?’，主要讲了自己学习NLG的一些方法及感悟，感兴趣的同学可以拜读一下。<br>

#### **Andrej Karpathy**
&ensp;&ensp;&ensp;&ensp;Andrej Karpathy是计算机视觉和深度学习领域的专家之一，毕业于斯坦福人工智能实验室，博士师从李飞飞教授，在谷歌大脑、DeepMind 实过习，与吴恩达一起共事，业界几大深度学习实验室都待过。他经常会在个人[twitter]()上以及[个人博客](http://karpathy.github.io/)上面分享一些关于深度学习相关想法和见解，比如前段时间他分享的[深度学习训练技巧](http://karpathy.github.io/2019/04/25/recipe/)受到了很多人的关注。看过他博客的个人介绍，可以发现，他在2011年到2015年学习期间，主要研究的方向是自然语言处理，它的一篇文章：[神奇的递归神经网络(RNN)](http://karpathy.github.io/2015/05/21/rnn-effectiveness/)是一篇相当不错的入门资料。并且还共享[文本生成](https://github.com/karpathy/char-rnn)的代码。

#### **万小军** 
&ensp;&ensp;&ensp;&ensp;[万小军](https://wanxiaojun.github.io/)是北京大学王选计算机研究所研究员，主要研究领域有自然语言处理，文本挖掘，人工智能。它是语言计算与互联网挖掘研究室（从属北京大学王选计算机科学技术研究所）的负责人。该研究室以自然语言处理技术、数据挖掘技术与机器学习技术为基础，对互联网上多源异质的文本大数据进行智能分析与深度挖掘，为互联网搜索、舆情与情报分析、写稿与对话机器人等系统提供关键技术支撑，并从事计算机科学与人文社会科学的交叉科学研究。 研究室当前研究内容包括：1）语义理解：研制全新的语义分析系统实现对人类语言（尤其是汉语）的深层语义理解；2）机器写作：综合利用自动文摘与自然语言生成等技术让机器写出高质量的各类稿件；3）情感计算：针对多语言互联网文本实现高精度情感、立场与幽默分析；4）其他：兴趣技术探索。<br>

### 干货学习资源
#### 文本生成资源大列表
&ensp;&ensp;&ensp;&ensp;[文本生成资源大列表](https://github.com/ChenChengKuan/awesome-text-generation),该资源主要整理列举了2018年EMNLP的优秀文本生成模型及应用案例（主要以Paper的形式给出）。其中主要包括：模型（GAN based、VAE based、Autoencoder based、Reinforcement learning based、Alternative decode objective、Tool and others）、应用（基于文本的强化学习、基于GAN的对抗学习等）。<br>

#### 文本生成必读的几篇文章
&ensp;&ensp;&ensp;&ensp;1、[Character based Recurrent Neural Network](https://github.com/karpathy/char-rnn)
&ensp;&ensp;&ensp;&ensp;该篇文章主要讲述了最基本的Char-RNN文本生成原理，具体如下图所示。以要让模型学习写出“hello”为例，Char-RNN的输入输出层都是以字符为单位。输入“h”，应该输出“e”；输入“e”，则应该输出后续的“l”。输入层我们可以用只有一个元素为1的向量来编码不同的字符，例如，h被编码为“1000”、“e”被编码为“0100”，而“l”被编码为“0010”。使用RNN的学习目标是，可以让生成的下一个字符尽量与训练样本里的目标输出一致。在图一的例子中，根据前两个字符产生的状态和第三个输入“l”预测出的下一个字符的向量为<0.1, 0.5, 1.9, -1.1>，最大的一维是第三维，对应的字符则为“0010”，正好是“l”。这就是一个正确的预测。但从第一个“h”得到的输出向量是第四维最大，对应的并不是“e”，这样就产生代价。学习的过程就是不断降低这个代价。学习到的模型，对任何输入字符可以很好地不断预测下一个字符，如此一来就能生成句子或段落。<br>
<div align=center>![image.png](https://upload-images.jianshu.io/upload_images/18628169-f3208db19bb7cb01.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/240)<br>

&ensp;&ensp;&ensp;&ensp;1、[A Deep Ensemble Model with Slot Alignment for Sequence-to-Sequence Natural Language Generation](https://arxiv.org/pdf/1805.06553.pdf)<br>
&ensp;&ensp;&ensp;&ensp;2、[SeqGAN: Sequence Generative Adversarial Nets with Policy Gradient](https://arxiv.org/pdf/1609.05473.pdf)<br>
&ensp;&ensp;&ensp;&ensp;3、[Generative Adversarial Text to Image Synthesis](https://arxiv.org/pdf/1605.05396.pdf)<br>




## 未完待续。。。


