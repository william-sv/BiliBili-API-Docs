###### BiliBili API接口
> 本文档基于BiliBili 网站的请求数据中获取到
> 本文档更新于2018年08月06日

- 获取栏目中的条目
   http://api.bilibili.com/archive_rank/getarchiverankbypartion?type=jsonp&tid=168&pn=1
   ###### 返回字段
   |返回值字段|字段类型|字段说明|
   |---|---|---|
   |code|int|code状态|
   |message|int|N/A|
   |ttl|int|N/A|
   |data|Object|返回的数据|

   ###### Data字段
   |返回值字段|字段类型|字段说明|
   |---|---|---|
   |archives|Object|N/A|
   |page|object|页码信息|

   ###### archives字段
   |返回值字段|字段类型|字段说明|
   |---|---|---|
   |aid|int|视频ID|
   |videos|int|N/A|
   |tid|int|栏目id|
   |tname|string|栏目名|
   |copyright|int|版权|
   |pic|string|视频poster|
   |title|string|视频名称|
   |attribute|int|N/A|
   |duration|int|N/A|
   |rights|Object|N/A|
   |stat|int|N/A|
   |dynamic|string|视频标签|
   |cid|int|N/A|
   |dimension|int|N/A|
   |play|int|播放量|
   |favorites|int|N/A|
   |video_review|int|N/A|
   |create|int|视频上传时间|
   |description|int|N/A|
   |mid|int|UP主id|
   |author|int|作者|
   |face|int|作者头像|

   ###### rights字段
   |返回值字段|字段类型|字段说明|
   |---|---|---|
   |bp|int|N/A|
   |elec|int|N/A|
   |download|int|N/A|
   |movie|int|N/A|
   |pay|int|N/A|
   |hd5|int|N/A|
   |no_reprint|int|N/A|
   |autoplay|int|N/A|

   ###### stat字段
   |返回值字段|字段类型|字段说明|
   |---|---|---|
   |aid|int|视频id|
   |view|int|观看量|
   |danmaku|int|弹幕数|
   |reply|int|评论|
   |favorite|int|N/A|
   |coin|int|币数|
   |share|int|分享数|
   |now_rank|int|现在排名|
   |his_rank|int|历史排名|
   |like|int|好评|
   |dislike|int|差评|

   ###### page字段
   |返回值字段|字段类型|字段说明|
   |---|---|---|
   |count|int|当前栏目item的总数|
   |num|int|当前返回的页码|
   |size|int|返回的item数|

- 栏目动态接口 （通过这个接口可以获取到Bilibili启用的栏目的tid）
  https://api.bilibili.com/x/web-interface/dynamic/total?jsonp=jsonp&callback=dynamic_total
  
  ###### 返回字段
  |返回值字段|字段类型|字段说明|
  |---|---|---|
  |code|int|接口状态|
  |message|int|N/A|
  |ttl|int|N/A|
  |data|Object|返回的数据|
  
- 
