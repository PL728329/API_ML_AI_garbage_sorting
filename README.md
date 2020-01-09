# 垃圾分类app产品需求文档

发布内容|2019-12-05
--|:--:|
|APP名称|垃圾分分看|
|文件现状|进行中|
|项目所有人|彭海晴|
|开发者|彭海晴|
|测试者|彭海晴|
- [20*20ppt文档下载](https://raw.githubusercontent.com/PL728329/API_ML_AI_garbage_sorting/master/%E5%9E%83%E5%9C%BE%E5%88%86%E5%88%86%E7%9C%8B.pptx)

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

## （八）需求列表与人工智能API

| 用户案例 | 对应功能 | 重要程度 |
:---:|:---:|:---:|
| 用户想快速分辨手中的垃圾为何类型 | 京东-垃圾分类识别功能 | 重要 |
| 用户想得到垃圾分类投放建议 | 京东-垃圾分类识别功能 | 重要 |
| 用户使用app时希望能更精准进行识别 | 百度-主体检测识别功能 | 次重要 |
| 用户想了解一些垃圾分类小常识 | 科普功能 | 次重要 |

### 具体应用场景
- 场景一：小海在家点了一份外卖小龙虾，里面配备了饮料、塑料手套、木筷子、勺子等其他食品和工具，小海开心的吃完外卖后，面对满桌的垃圾陷入沉思，这些垃圾该如何分类呢？于是小海点开垃圾分分看，通过图片上传分辨垃圾类型，很快就将桌上的垃圾清理完毕了。（垃圾分类识别功能）

- 场景二：小海喜欢在上班的路上买瓶装咖啡来喝，但是每次喝完之后，小海虽然知道瓶子属于什么类型的垃圾，但总是很纠结要如何投放进垃圾桶才能减少环卫工人的工作量，于是她点开了垃圾分分看，将瓶子的图片上传至app上，很快，app给小海识别出了瓶子属于什么类型的垃圾，并且给了小海如何处理这类垃圾的建议，小海根据建议，整理好了垃圾，投进了垃圾桶里。（垃圾分类识别功能）

- 场景三：小海的父亲是个老顽固，对最近推行的垃圾分类政策十分不满，认为没有必要，也不愿意去学习如何进行垃圾分类。小海为此特地在父亲的手机上安装了“垃圾分分看”app，帮助父亲进行垃圾分类，一开始小海的父亲还对垃圾分类十分排斥，但在使用“垃圾分分看”app后，在其科普功能里面看了不少关于垃圾分类的知识后，逐渐就不那么排斥垃圾分类了。（科普功能）

# 原型
## （九）使用者交互与设计（axure产品原型）
- [原型文档展示](https://pl728329.github.io/api_prototype/)
- [原型文档下载区](https://github.com/PL728329/api_prototype)

#### 交互及界面设计
- **登录界面**-用户登录时所看到的界面

![登录页面](https://github.com/PL728329/API_ML_AI_garbage_sorting/blob/master/images/%E7%99%BB%E5%BD%95%E9%A1%B5%E9%9D%A2.png)

- **个人页面**-app内的个人模块

![个人页面](https://github.com/PL728329/API_ML_AI_garbage_sorting/blob/master/images/%E4%B8%AA%E4%BA%BA%E9%A1%B5%E9%9D%A2.png)

- **分类识别页面**-用户在此处可根据自己的需求选择识别类型

![分类识别页面](https://github.com/PL728329/API_ML_AI_garbage_sorting/blob/master/images/%E5%88%86%E7%B1%BB%E8%AF%86%E5%88%AB%E9%A1%B5%E9%9D%A2.png)

- **分类识别页面-拍照识别**

![拍照识别](https://github.com/PL728329/API_ML_AI_garbage_sorting/blob/master/images/%E5%88%86%E7%B1%BB%E8%AF%86%E5%88%AB-%E6%8B%8D%E7%85%A7%E8%AF%86%E5%88%AB.png)

- **分类识别页面-文本识别**

![文本识别](https://github.com/PL728329/API_ML_AI_garbage_sorting/blob/master/images/%E5%88%86%E7%B1%BB%E8%AF%86%E5%88%AB-%E6%96%87%E6%9C%AC%E8%AF%86%E5%88%AB.png)

- **分类识别页面-语音识别**

![语音识别](https://github.com/PL728329/API_ML_AI_garbage_sorting/blob/master/images/%E5%88%86%E7%B1%BB%E8%AF%86%E5%88%AB-%E8%AF%AD%E9%9F%B3%E8%AF%86%E5%88%AB.png)

- **科普知识页面**-用户可在此处查阅垃圾分类知识以及相关环保类科普文章

![科普知识页面](https://github.com/PL728329/API_ML_AI_garbage_sorting/blob/master/images/%E7%A7%91%E6%99%AE%E7%9F%A5%E8%AF%86%E9%A1%B5%E9%9D%A2.png)

- **产品结构图**

![产品结构图](https://github.com/PL728329/API_ML_AI_garbage_sorting/blob/master/images/APP%E4%BA%A7%E5%93%81%E7%BB%93%E6%9E%84%E5%9B%BE.png)

- **功能结构图**

![功能结构图](https://github.com/PL728329/API_ML_AI_garbage_sorting/blob/master/images/APP%E5%8A%9F%E8%83%BD%E7%BB%93%E6%9E%84%E5%9B%BE.png)

- **信息结构图**

![信息结构图](https://github.com/PL728329/API_ML_AI_garbage_sorting/blob/master/images/APP%E4%BF%A1%E6%81%AF%E7%BB%93%E6%9E%84%E5%9B%BE.png)

- **产品流程图**

![产品流程图](https://github.com/PL728329/API_ML_AI_garbage_sorting/blob/master/images/APP%E4%BA%A7%E5%93%81%E6%B5%81%E7%A8%8B%E5%9B%BE.png)

## （十）API使用（使用水平）
1. 京东人工智能开放平台-垃圾分类识别api
- 接口描述：垃圾分类识别API可用于解决令人头疼的垃圾分类问题。基于京东AI庞大商品识别能力进行拓展，提供数亿种生活垃圾的辨识和分类建议，支持多模态（图片、文字、语音）搜索，支持快速场景搭建。
- **图片识别**
- 接口地址：https://aiapi.jd.com/jdai/garbageVoiceSearch
- 请求方式:https post postaiapi.jd.com/jdai/garbageImageSearch
- 输入：
```
#!/usr/bin/python
# -*- coding: utf-8 -*-
# 本代码仅供参考，请根据实际情况进行调整
import wx_sdk

url = 'https://aiapi.jd.com/jdai/garbageImageSearch'
bodyStr = '{ 	"cityId":"310000", 	"imgBase64":"XXXXXX"}' #body中的内容
params = { 
    'appkey' : '38981eb926e28ef6d229284ebd2939bb',
    'secretkey' : 'your secretKey'
}

response = wx_sdk.wx_post_req( url, params, bodyStr=bodyStr )
print( response.text )

```
- 输出：
```
Status Code: 200
Time：1262ms
Date：Tue 10 Dec 2019 17:24:16 GMT
Body：
{
    "code": "10000",
    "charge": true,
    "remain": 4997,
    "remainTimes": 4997,
    "remainSeconds": -1,
    "msg": "查询成功,扣费",
    "result": {
        "status": 0,
        "message": "success",
        "garbage_info": [
            {
                "cate_name": "湿垃圾",
                "city_id": "310000",
                "city_name": "上海市",
                "confidence": 0.9550853795837226,
                "garbage_name": "咖啡/奶茶",
                "ps": "投放建议：容器与外包装为可回收物"
            }
        ]
    }
}
```

- 京东人工智能开放平台垃圾分类识别测试结果：

- 单一物体识别：输入一张有关于饮料的照片，输出一个置信度最高的识别结果。
- 输入图片：
![输入单一物体图片](https://github.com/PL728329/API_ML_AI_garbage_sorting/blob/master/images/1039f5750243da9e5755808882aa4b89.jpg)
- 输出结果：
![单一物体输出结果](https://github.com/PL728329/API_ML_AI_garbage_sorting/blob/master/images/%E5%A5%B6%E8%8C%B6-%E8%AF%86%E5%88%AB.png)

- 多物体识别：输入一张包含多样物品的照片，输出一个置信度最高的识别结果。
- 输入图片：
![输入多物体图片](https://github.com/PL728329/API_ML_AI_garbage_sorting/blob/master/images/1369025_131058903000_2.jpg)
- 输出结果：
![多物体输出结果](https://github.com/PL728329/API_ML_AI_garbage_sorting/blob/master/images/%E9%87%8E%E9%A4%90-%E8%AF%86%E5%88%AB.png)
- 多物体照片一样可以进行识别，只是置信度相对于单一物体来说下降不少。

---

#### 2. 天行数据-垃圾分类api
- 接口描述：
- 垃圾分类成为城市生活新时尚，但也成为大家的新烦恼。本API接口支持查询绝大部分中常见或不常见的生活废弃物的垃圾类型，并给出相关物品和分类建议。对于相关名字不同物品的废弃物，也分别给出不同的分类。目前已有近万条废弃物种类数据，针对用户输入的复杂长尾词也有智能预判机制。同时系统会根据查询结果不断增加新的数据，以及根据政策和指导建议优化分类。
- API文档：[垃圾分类api](https://www.tianapi.com/apiview/97)

##### 文本识别
- 接口地址：http://api.tianapi.com/txapi/lajifenlei/index
- 请求方式：GET/POST
- 支持协议：HTTP/HTTPS
- 返回格式：UTF8 JSON

- 输入：
```
# -*- coding: utf-8 -*-
import sys, urllib, urllib2, json

url = 'http://api.tianapi.com/txapi/lajifenlei/index?key=APIKEY&word=眼镜'

req = urllib2.Request(url)

resp = urllib2.urlopen(req)
content = resp.read()
if(content):
    print(content)
```
- 输出：
```
Response Header:
HTTP/1.1 200 OK
Server: nginx
Date: Mon, 16 Dec 2019 06:43:37 GMT
Content-Type: application/json;charset=utf8
Transfer-Encoding: chunked
Connection: keep-alive
Access-Control-Allow-Origin: *
Access-Control-Allow-Methods: POST,GET,OPTIONS
Access-Control-Allow-Headers: Content-Type,Access-Control-Allow-Headers,X-Requested-with,Origin
TianAPI-Cache: OK
Vary: Accept-Encoding
Via: 1008


Response Body:
{
  "code": 200,
  "msg": "success",
  "newslist": [
    {
      "name": "太阳眼镜",
      "type": 3,
      "aipre": 0,
      "explain": "干垃圾即其它垃圾，指除可回收物、有害垃圾、厨余垃圾（湿垃圾）以外的其它生活废弃物。",
      "contain": "常见包括砖瓦陶瓷、渣土、卫生间废纸、猫砂、污损塑料、毛发、硬壳、一次性制品、灰土、瓷器碎片等难以回收的废弃物",
      "tip": "尽量沥干水分；难以辨识类别的生活垃圾都可以投入干垃圾容器内"
    },
    {
      "name": "智能眼镜",
      "type": 0,
      "aipre": 0,
      "explain": "可回收垃圾是指适宜回收、可循环利用的生活废弃物。",
      "contain": "常见包括各类废金属、玻璃瓶、易拉罐、饮料瓶、塑料玩具、书本、报纸、广告单、纸板箱、衣服、床上用品、电子产品等",
      "tip": "轻投轻放；清洁干燥，避免污染，费纸尽量平整；立体包装物请清空内容物，清洁后压扁投放；有尖锐边角的、应包裹后投放"
    },
```
- 此处输出结果有多个，因篇幅太长只放部分到文档内。
---

#### 3.艾科瑞特（iCREDIT）——可回收垃圾分类识别
- 描述：支持城市级垃圾分类识别，智能干湿垃圾分类识别，可回收垃圾识别分类、电子垃圾识别回收分类。
- API文档：[可回收垃圾分类识别api](https://market.aliyun.com/products/57126001/cmapi032724.html#sku=yuncode2672400001)

- 调用地址：http://rubbish.market.alicloudapi.com/ai_market/ai_image_universal/rubbish/v1
- 请求方式：POST
- 返回类型：JSON

- 输入：
```
# -*- coding: UTF-8 -*-
# !/usr/bin/python3
# 版权所有 © 艾科瑞特科技
# 艾科瑞特（iCREDIT）-让企业业绩长青
# 预知更多业绩长青，请与我们联系
# 联系电话：0532-88984128
# 联系邮箱：market@itruth.xin

import urllib
import urllib.request
import time
import base64

#UUID采用当前程序运行时间，用于防止重放攻击，开发者可根据自己需求，自定义字符串
UUID = str(time.time())
#API产品路径
host = 'http://rubbish.market.alicloudapi.com'
path = '/ai_market/ai_image_universal/rubbish/v1'
#阿里云APPCODE
appcode = '你的阿里云APPCODE' 
bodys = {}
url = host + path

#内容数据类型，如：0，则表示BASE64编码；1，则表示图像文件URL链接

#启用BASE64编码方式进行识别
#内容数据类型是BASE64编码
#f = open(r'图片文件', 'rb')
#contents = base64.b64encode(f.read())
#f.close()
#bodys['IMAGE'] = contents
#bodys['IMAGE_TYPE'] = '0'

#启用URL方式进行识别
#内容数据类型是图像文件URL链接
bodys['IMAGE'] = '图片URL链接'
bodys['IMAGE_TYPE'] = '1'

post_data = urllib.parse.urlencode(bodys).encode('utf-8')
request = urllib.request.Request(url, post_data)
request.add_header('Authorization', 'APPCODE ' + appcode)
request.add_header('Content-Type', 'application/x-www-form-urlencoded; charset=UTF-8')
request.add_header('X-Ca-Nonce', UUID)
response = urllib.request.urlopen(request)
content = response.read()
if (content):
    print(content.decode('utf-8'))
```
- 输出：
```
{
    "METAL":"99.99",              #METAL
    "GLASS":"08.99",              #GLASS
    "PLASTIC":"66.99",            #PLASTIC
    "PAPER":"12.99",              #PAPER
    "OTHER":"88.99"               #OTHER
}
```
- 可回收垃圾分类识别测试结果：
- [测试结果](http://nfunm069.gitee.io/icredit)


#### 4.百度AI开放平台——图像主体检测api
- 描述：检测出图片主体的坐标位置，可使用该接口裁剪出图像主体区域，配合图像识别接口提升识别精度。广泛适用于美图类app、辅助智能识图等业务场景中。
- API文档：[图像主体检测api](https://ai.baidu.com/tech/imagerecognition/object_detect)

- 请求URL：https://aip.baidubce.com/rest/2.0/image-classify/v1/object_detect
- HTTP 方法：POST

- 输入：
```
# encoding:utf-8

import requests
import base64

'''
图像主体检测
'''

request_url = "https://aip.baidubce.com/rest/2.0/image-classify/v1/object_detect"
# 二进制方式打开图片文件
f = open('[本地文件]', 'rb')
img = base64.b64encode(f.read())

params = {"image":img,"with_face":1}
access_token = '[调用鉴权接口获取的token]'
request_url = request_url + "?access_token=" + access_token
headers = {'content-type': 'application/x-www-form-urlencoded'}
response = requests.post(request_url, data=params, headers=headers)
if response:
    print (response.json())
```
- 输出：
```
HTTP/1.1 200 OK
x-bce-request-id: 73c4e74c-3101-4a00-bf44-fe246959c05e
Cache-Control: no-cache
Server: BWS
Date: Tue, 18 Oct 2016 02:21:01 GMT
Content-Type: application/json;charset=UTF-8
{
  "log_id": 895582300,
  "result": {
    "width": 486,
    "top": 76,
    "left": 134,
    "height": 394
  }
}
```
- 图像主体检测识别测试结果：
![测试结果](https://github.com/PL728329/API_ML_AI_garbage_sorting/blob/master/images/%E4%B8%BB%E4%BD%93%E6%A3%80%E6%B5%8B.png)

- 图像主体检测测试代码：
![图像主体检测测试代码](https://github.com/PL728329/API_ML_AI_garbage_sorting/blob/master/images/%E7%89%A9%E4%BD%93%E4%B8%BB%E4%BD%93%E6%A3%80%E6%B5%8B.png)

---
## （十一）API使用比较分析
- 京东垃圾分类识别api：
  1. 支持多种模态搜索；
  2. 可以针对不同城市要求，针对识别结果给出投放建议；
  3. 依托京东商城海量商品，支持数亿商品识别并提供建议；
  4. 暂时免费调用，日调用量限制5000次/日，QPS（每秒查询率）限制：5；
- 天行数据垃圾分类api：
  1. 目前已有几千条废弃物种类；
  2. 同样支持多模态搜索；
  3. api可以直接打包生成小程序；
  4. 会员制计费，每次调用价格约为0.0001元/次；
  5. [天行数据价格](https://www.tianapi.com/apiview/107#apiprice)

- 聚合数据垃圾分类api：
  1. 支持实时热门垃圾搜索；
  2. 查询模式分“清晰”、“模糊”两种；
  3. 拥有分类说明；
  4. 每次调用价格约为0.002元/次；
  5. [聚合数据价格](https://www.juhe.cn/docs/api/id/375)

- iCREDIT垃圾分类api：
  1. 更偏向于可回收垃圾分类识别；
  2. 每次调用价格约为0.0059元；
  3. [iCREDIT价格](https://market.aliyun.com/products/57126001/cmapi032724.html#sku=yuncode2672400001)

- 百度AI开放平台：
  1. 可以进行图像识别辅助，辅助图像识别提高精度；
  2. 开通后调用量无限制，QPS（每秒查询率）限制：10，调用价格按梯度计算；
  3. [百度开放平台价格](https://ai.baidu.com/ai-doc/IMAGERECOGNITION/rk3bcxa9e)

- 根据使用感、文档完整度、调用价格这几方面来看，“垃圾分分看”这一个APP暂时会使用京东垃圾分类识别api作为APP内垃圾分类识别功能的接口，原因如下：
  1. 依托京东商城海量商品，支持数亿商品识别，相对于别的数据接口来说，其后台所拥有的数据更丰富、更全面；
  2. 支持多模态搜索，使用时有更多选择；
  3. 给出的产品文档基本完整，并且其可以针对不同城市要求，针对识别结果给出投放建议（目前只支持上海地区）
- 而在APP内的垃圾分类功能中，还将会使用百度开放平台的图像主体检测api来辅助垃圾分类识别功能，原因如下：
  1. 给出的API文档相对完整，上手速度较快；
  2. 百度AI开放平台知名度相对较高；

## （十二）人工智能概率性
- 垃圾分类api：
  1. 在图片杂物过多时，不能精准识别图内单独某个物品，各项置信度都很低，没办法进行垃圾分类识别；
- 例子：
![识别置信度低](https://github.com/PL728329/API_ML_AI_garbage_sorting/blob/master/images/%E8%B4%AD%E7%89%A9-%E8%AF%86%E5%88%AB.png)

- 解决办法：运用图像主体检测api加以辅助，缩小识别范围，提高精确度。
- 图像主体检测api：
  1. 图片内出现较多物体时，会存在无法检测主体的情况，可能会达不到预想的要求；
- 例子：
![主体检测](https://github.com/PL728329/API_ML_AI_garbage_sorting/blob/master/images/%E8%B4%AD%E7%89%A9-%E6%A3%80%E6%B5%8B.png)

- 解决办法：暂时没找到解决办法，待定。

## （十三）使用后风险报告
- 垃圾分类识别api：
  1. 未来发展性：中国正全面启动生活垃圾分类工作，虽然现在只是在某部分城市作为试点进行推行，但在此大环境之下，全面推行垃圾分类只是时间问题。目前推出垃圾分类识别api的开放平台还不算多，而已经推出的垃圾分类识别api数据也还需要进一步的丰富与完善，因此垃圾分类识别api还是很有前景的。
  2. 市场竞争程度：目前只有为数不多的平台专门推出垃圾分类识别api，但可能等到全面推行垃圾分类时，垃圾分类识别api的热度会提升，因此垃圾分类识别api的市场竞争还是十分激烈的。



