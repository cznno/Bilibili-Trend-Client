[toc]

# 参数分析

## Up 主信息

```
https://space.bilibili.com/ajax/member/

getSubmitVideos?

mid=423895&

pagesize=100&

page=4
```


| 参数              | 作用                  |
| --------------- | ------------------- |
| getSubmitVideos | 获取投稿视频              |
| mid             | 用户 UID              |
| pagesize        | 每页返回的数量，最大100       |
| page            | 显示页内容，可以配合 pagesize |

## 从视频中获取 UP 信息
```
https://api.bilibili.com/x/web-interface/
card?
callback=jQuery17203315846063444545_1519535784552&
mid=306805&
jsonp=jsonp&
```

## 搜索

```
https://search.bilibili.com/

api/

search?

search_type=bili_user

&keyword=%E7%8E%8B%E8%80%81%E8%8F%8A
```

| 参数          | 作用                     |
| ----------- | ---------------------- |
| keyword     | 需要搜索的用户                |
| search_type | ALL:综合搜索  bili_user:用户 |

## 分区信息

```
https://api.bilibili.com/x/web-interface/ranking/
region?
callback=jQuery172013842556841451836_1519392349252&
rid=13&
day=7&
jsonp=jsonp
```

```
https://www.bilibili.com/

index/

rank/

all-07-119.json
```

| 参数       | 作用            |
| -------- | ------------- |
| callback | 一段代码 + 时间戳        |
| rid      | 分区信息，下面进行详细分析 |
| day      | 应该是日期，无法更改    |
| jsonp    | jsonp         |
| all-07-119.json    |     见下   |
| 7/0/3    |     7天内，加0表示十分钟更新，不加一天更新一次   |
| 119      |     分区编号，见下   |

## rid 详解

|    值    |    分区     |
| :-----: | :-------: |
|    1    |    动画     |
|    3    |    音乐     |
|    4    |    游戏     |
|    5    |    综艺     |
|   11    |    电视剧    |
|   13    |    番剧     |
|   36    |    科技     |
|   119   |    鬼畜     |
|   129   |    舞蹈     |
|   23    | 国产电影/华语电影 |
|   155   |    时尚     |
|   160   |    生活     |
| 165/166 |    广告     |
|   177   |    纪录片    |
|   181   |    影视     |
|         |           |
|         |           |

#### 游戏分区

|  值   |  分区   |
| :--: | :---: |
|  17  | 单机联机  |
|  19  | Mugen |
|  65  | 网络游戏  |
| 121  |  GMV  |
| 136  |  音游   |
| 171  | 电子竞技  |
| 172  | 手机游戏  |
| 173  | 桌游棋牌  |
|      |       |

#### 舞蹈分区

|  值   |  分区   |
| :--: | :---: |
|  20  |  宅舞   |
| 154  | 三次元舞蹈 |
| 156  | 舞蹈教程  |
|      |       |
|      |       |

#### 生活分区

|  值   |  分区  |
| :--: | :--: |
|  21  |  日常  |
|  75  | 动物圈  |
|  76  | 美食圈  |
| 138  |  搞笑  |
| 161  |  手工  |
| 162  |  绘画  |
| 163  |  运动  |
| 174  |  其他  |
| 175  | ASMR |

#### 鬼畜分区

|  值   |     分区     |
| :--: | :--------: |
|  22  |    鬼畜调教    |
|  26  |    音MAD    |
|  54  | OP/ED/OST  |
| 126  | 人力VOCALOID |
| 127  |    教程演示    |

#### 电影分区

|  值   |    分区    |
| :--: | :------: |
|  83  | 电影/放映厅电影 |
| 145  |   欧美电影   |
| 146  |   日本电影   |
| 147  |   国产电影   |
|      |          |

#### 动画分区

|  值   |    分区    |
| :--: | :------: |
|  24  | MAD·AMV  |
|  25  |  MMD·3D  |
|  27  |    综合    |
|  47  | 短片·手书·配音 |
|      |          |

#### 音乐分区

|  值   |      分区       |
| :--: | :-----------: |
|  28  |     原创音乐      |
|  29  |     三次元音乐     |
|  30  | VOCALOID·UTAU |
|  31  |      翻唱       |
|  59  |      演奏       |
| 130  |     音乐选集      |
|      |               |

#### 番剧分区

|  值   |  分区  |
| :--: | :--: |
|  32  | 完结动画 |
|  33  | 连载动画 |
|  51  |  资讯  |
| 152  | 官方延伸 |
|      |      |

#### 电视剧分区

|     值     |  分区  |
| :-------: | :--: |
|    186    | 港台剧  |
| 185/34/15 | 国产剧  |
|    187    | 海外剧  |

#### 科技分区

|  值   |   分区    |
| :--: | :-----: |
| 124  | 趣味科普人文  |
|  39  | 演讲• 公开课 |
|  95  |   数码    |
|  96  |   星海    |
|  98  |   机械    |
| 122  | 野生技术协会  |
| 176  |   汽车    |
|      |         |

#### 纪录片分区

|  值   |   分区   |
| :--: | :----: |
|  36  | 趣味科普人文 |
|  37  |  人文历史  |
|      |        |

#### 娱乐分区

|  值   |   分区    |
| :--: | :-----: |
|  71  |   综艺    |
| 131  | Korea相关 |
|      |         |

#### 影视分区

|   值    |  分区   |
| :----: | :---: |
|   82   | 预告 资讯 |
|   85   |  短片   |
| 86/128 |  特摄   |
|  137   |  明星   |
|  182   | 影视杂谈  |
|  183   | 影视剪辑  |
|  184   | 预告 资讯 |

#### 国创分区

|    值    |   分区   |
| :-----: | :----: |
|   153   |  国产动画  |
| 167/168 | 国产原创相关 |
|   169   |  布袋戏   |
|   170   |   资讯   |
|         |        |
|         |        |

#### 时尚分区

|  值   |  分区  |
| :--: | :--: |
| 158  |  服饰  |
| 157  |  美妆  |
| 159  |  资讯  |
| 164  |  健身  |
|      |      |
|      |      |

#### 纪录片分区

|  值   |   分区   |
| :--: | :----: |
| 178  |  科学探索  |
| 179  |  热血军事  |
| 180  | 舌尖上的旅行 |
|      |        |
|      |        |
|      |        |
