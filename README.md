# 垃圾分类app产品需求文档

发布内容|2019-12-05
--|:--:|
|APP名称|垃圾分分看|
|文件现状|进行中|
|项目所有人|彭海晴|
|开发者|彭海晴|
|测试者|彭海晴|

# 价值主张设计
## （一）背景
- 2019年起全国地级及以上城市将全面启动生活垃圾分类工作，而在2019年7月份，上海作为全国第一个试点，开始进行垃圾分类。
- 垃圾分类对于中国大众来说可以说是一次全新的尝试，此前我们从未尝试过进行垃圾分类，因此可能会出现以前情况：
   * 部分人弄不懂垃圾该如何分类。
   * 部分人不理解为何进行垃圾分类，不理解垃圾分类的好处，对这方面的基础知识薄弱。

## （二）加值宣言
- 2019年7月份，上海作为全国第一个试点，开始实行国人第一次垃圾分类，目前来说，由于是初次实行垃圾分类，在手中的垃圾到底是个什么类型的垃圾的问题上，难倒了许多人。
- 于是有人开始提出意见：是否可以通过机器来帮助我们更快更好的进行垃圾分类呢？
- 基于现状，现将会使用京东人工智能开放平台的垃圾分类识别api和百度ai开放平台的图像主体检测api对现有的产品进行加值和优化。
- **主要**
   * 运用垃圾分类识别api，用户可选择通过传入单个垃圾名称进行文本形式的查询，也可通过传入图片进行图片形式的查询，也可以传入语音进行语音形式的查询。
- **辅助**
   * 运用百度ai开放平台的图像主体检测裁剪出图像主体区域，配合垃圾分类识别接口提升识别精度。
   * 导入垃圾分类的各类知识，在帮助用户进行垃圾分类的基础上也对用户进行科普，提高全民垃圾分类的意识。

## （三）核心价值（最小可行性产品）
- 着重于当前最紧迫的需求，解决用户垃圾分类不准确、分类花费时间长的问题，提供给用户快速识别垃圾类型的基础服务。

## （四）目的
- 一个帮你进行垃圾分类的贴心APP——“垃圾分分看”

## （五）目标
- 前期目标：
   1. 识别该物体属于何类型垃圾。
   2. 识别后给予用户该类型垃圾的投放建议。
   3. 给用户科普垃圾分类知识，提高用户对这方面的知识储备。

- 后期目标（构思想法）：
   1. 目前没有，后续补充。


## （六）用户
- 正在进行垃圾分类的城市/农村居民、环保爱好者。

## （七）用户痛点
- 场景一：大众对各类垃圾归属何类型了解不深，且垃圾众多，在丢垃圾时不知如何正确分类。为了分辨手中的垃圾花费大量时间。
- 场景二：部分人群垃圾分类错误，环卫工人在处理垃圾时需重新分类，增加环卫工人工作量。
- 场景三：部分人不理解垃圾分类的必要性，比较排斥，给垃圾分类的普及与推行增加难度。


## （八）用户需求（使用的人工智能要反映到列表当中）

| 用户案例 | 对应功能 | 重要程度 |
:---:|:---:|:---:|
| 用户想快速分辨手中的垃圾为何类型 | 垃圾分类识别功能 | 重要 |
| 用户想得到垃圾分类投放建议 | 垃圾分类识别功能 | 重要 |
| 用户想了解一些垃圾分类小常识 | 科普功能 | 次重要 |

### 具体应用场景
- 场景一：小海在家点了一份外卖小龙虾，里面配备了饮料、塑料手套、木筷子、勺子等其他食品和工具，小海开心的吃完外卖后，面对满桌的垃圾陷入沉思，这些垃圾该如何分类呢？于是小海点开垃圾分分看，通过图片上传分辨垃圾类型，很快就将桌上的垃圾清理完毕了。（垃圾分类识别功能）

- 场景二：小海喜欢在上班的路上买瓶装咖啡来喝，但是每次喝完之后，小海虽然知道瓶子属于什么类型的垃圾，但总是很纠结要如何投放进垃圾桶才能减少环卫工人的工作量，于是她点开了垃圾分分看，将瓶子的图片上传至app上，很快，app给小海识别出了瓶子属于什么类型的垃圾，并且给了小海如何处理这类垃圾的建议，小海根据建议，整理好了垃圾，投进了垃圾桶里。（垃圾分类识别功能）

- 场景三：小海的父亲是个老顽固，对最近推行的垃圾分类政策十分不满，认为没有必要，也不愿意去学习如何进行垃圾分类。小海为此特地在父亲的手机上安装了“垃圾分分看”app，帮助父亲进行垃圾分类，一开始小海的父亲还对垃圾分类十分排斥，但在使用“垃圾分分看”app后，在其科普功能里面看了不少关于垃圾分类的知识后，逐渐就不那么排斥垃圾分类了。（科普功能）

# 原型
## （九）使用者交互与设计（axure产品原型）
- [原型文档展示](http://nfunm069.gitee.io/prototype)
- [原型文档下载区](https://gitee.com/NFUNM069/prototype)
## （十）产品/功能/信息/流程结构图
