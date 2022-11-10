# Android-security-paper
本项目主要是对Android安全文章阅读的笔记收集整理，帮助硕博和从业人员快速阅读论文，了解领域的知识，论文的pdf获取，微信公众号输入索引号 或加入知识星球

## 研究领域

### 1.Android恶意应用检测

**1.《安卓恶意软件检测方法综述》（中国科学（信息科学）CCF-A-2020）**

论文简介：今天介绍2020年西安交通大学范铭教授团队在中国科学（信息科学）发表的论文《安卓恶意软件检测方法综述》。通过本篇综述，研究者可以快速了解近些年的Android恶意软件检测方面的相关发展，本文绍了恶意软件检测所面临的问题与挑战,然后综述了近些年的恶意软件检测所使用的数据集信息以及相关方法,将现有方法分为了基于特征码、基于机器学习以及基于行为3大类,并针对各方法所使用的技术进行了归纳总结,全面比较和分析了不同技术的优缺点.最后,结合我们自身在恶意软件检测方面的研究基础对未来的研究方向和面临的挑战进行了探索与讨论.

**2.Checking app behavior against app descriptions（2014-ICSE）**

论文简介：该论文是14年比较老的一篇论文，主要研究Android恶意应用检测，通过检测Android恶意应用的API的情况和恶意应用的描述，来去检测恶意应用的一致性。这里想到和当下动静态检测android应用的api和检测应用隐私文本的描述来检测应用的合规性，有相同的思想。

**3.Attention-CNN在恶意代码检测中的应用研究 （计算机科学与探索 CCF-B-2020）**

论文简介：该论文是2020年Android恶意代码检测的相关论文，该论文更好地提取恶意代码特征以及掌握恶意代码的行为,提出了基于注意力机制的Attention-CNN恶意代码检测模型。首先结合卷积神经网络（CNN）和注意力机制,构建了Attention-CNN恶意代码检测模型;然后将恶意代码转化为灰度图像作为模型输入,通过对Attention-CNN模型训练及测试得到恶意代码对应的注意力图以及检测结果;最终将从恶意代码注意力图中提取的重要字节序列用于人工分析,以揭示恶意代码的相关行为，而且从注意力图中提取的重要字节序列能够有效减轻人工分析的负担,获取恶意代码的相关行为,同时弥补了灰度图形式的恶意代码检测的不可解释性。

**4. InterDroid：面向概念漂移的可解释性Android恶意软件检测方法 (计算机研究与发展 CCF-A-2021）**

论文简介：针对Android恶意软件检测存在特征引入过程主观性高、特征选择过程可解释性差、训练模型检测效果不具备时间稳定性的问题，提出了一种面向概念漂移的可解释性Android恶意软件检测方法InterDroid，并通过实验证明 InterDroid筛选出的特征组合具备稳定性与可解释性。

**5. 代码向量深度学习的恶意 Android 应用检测方法（计算机应用研究 CCF-C-2021）**

论文简介：目前针对恶意Android应用的静态检测方法大多基于对病毒哈希值的分析与匹配,无法迅速检测出新型恶意Android应用及其变种,为了降低现有静态检测的漏报率,提高对新型恶意应用的检测速度,提出一种通过深度网络融合模型实现的恶意Android应用检测方法。首先提取反编译得到的Android应用核心代码中的静态特征,随后进行代码向量化处理,最后使用深度学习网络进行分类判别。该方法实现了对恶意应用高准确度的识别,经过与现存方法的对比分析,验证了该方法在恶意代码检测中的优越性。

**6. 基于 API 和 Permission 的 Android 恶意软件静态检测方法研究（计算机应用与软件 CCF-C-2020）**

论文简介：本文提出一种Android恶意软件静态检测方法。对收集到的训练集中的所有APK文件进行静态反编译,提取其中的静态信息;对静态信息中的API和Permission进行统计学分析,得到API和Permission在恶意APK和正常APK中的使用率;根据它们的使用率确定基准API和Permission集合,将每一个APK转换成可参与计算的关于API和Permission的特征向量;利用改进的k-NN分类器,对待检测的APK进行分类判定。实验结果表明,该方法可以有效地对APK进行恶意分类。

**7. 基于 API 配对的 Android 恶意应用检测 （ 西北工业大学学报   北大中文核心-2020）**

论文简介：针对基于Android应用程序申请权限的检测过于粗粒度的问题,提出了基于敏感应用程序编程接口（application program interface,API）配对的恶意应用检测方法。通过反编译应用程序提取危险权限对应的敏感API,将敏感API两两配对分别构建恶意应用无向图与良性应用无向图,再根据恶意应用和良性应用在敏感API调用上的差异分配相同边不同的权重,以此检测Android恶意应用。实验结果表明,提出的方法可以有效地检测出Android恶意应用程序,具有现实意义。

### 2.Android漏洞挖掘研究

**1.identity Confusion in WebView-based Mobile App-in-app Ecosystems（USENIX CCF-A-2022）**

论文简介：这是今年复旦大学计算机科学技术学院杨珉教授领衔的系统与软件安全实验室发表的论文，目前荣获网络安全国际顶尖学术会议31st USENIX Security Symposium杰出论文奖，论文主要关注于当前移动端小程序上面存在的漏洞问题，并展示了一种漏洞原理——身份混淆漏洞，通过混淆子应用程序的身份来获得特权API，然后集合WebView的加载机制，可以产生钓鱼、数据泄露、权限提升等漏洞。

### 3.Android混淆技术检测

### 4.Android脱壳技术研究

**1.Things You May Not Know About Android (Un)Packers: A Systematic Study based on Whole-System Emulation（NDSS CCF-A-2018）**

论文简介：今天介绍比较早的论文，2018年NDSS上的顶会论文，该论文提出了一个基于仿真器的脱壳机DroidUnPack, 该工具可以有效的进行脱壳，并且论文中的数据集也值得借鉴，论文描述了当前恶意应用加壳的现状。

**2.Happer: Unpacking Android Apps via a Hardware-Assisted Approach（S&P CCF-A 2021)**

论文简介：

该论文是香港理工大学罗夏朴教授发表在42届S&P顶会的论文，论文主要讲述硬件辅助的脱壳方案，特色主要在监控打包行为，并识别打包行为选择合适的策略脱壳，这种极大的应对了当前大量的环境检测问题，并提高了脱壳效率。
论文中团队共发现了27中打包行为分成10个类别：
（1）反调试类
<br>
（2）反模拟器类
<br>
（3）反动态插桩DBI类（比如反frida等）
<br>
（4）时间检测类
<br>
（5）系统API hook类（例如APP中通过hook write open等系统函数来进行对抗脱壳）
<br>
（6）动态加载类
<br>
（7）动态Dex修改类 （填充抽取壳）
<br>
（8）动态运行时对象修改类 （偏移抽取壳）
<br>
（9）Dex碎片化
<br>
（10）JIN转换 （例如java2c dex-vmp）

### 5.Android隐私合规研究

### 6.Android静态分析


未完待续...

注意：知识星球的论文编号对应与github上的顺序，例如序号1-1，对应github中Android恶意检测的序号1

### Contribute

本项目是由国内各大高校的硕博、安全从业人员、移动安全爱好者进行维护，相关的资料和笔记存放于知识星球，欢迎各位加入！

![image-20220902160158837](image/1.png)

考虑加群的广告号太多，需要加微信群朋友，加小编微信，回复:安全后厨

![640](https://tva3.sinaimg.cn/wap360/006jP03Oly1h7zufjtez2j30tu14fjur.jpg)

