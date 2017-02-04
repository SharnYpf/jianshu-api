# 爬取简书中的文章保存至 MySQL 并生成 API 
基于 **python 2.7** 和 **django 1.9**

简书 API 测试地址 : [http://222.24.63.118:8080/](http://222.24.63.118:8080/)

* [爬取简书全站文章并生成 API（一）](http://www.jianshu.com/p/c546c175b763)
* [爬取简书全站文章并生成 API（二）](http://www.jianshu.com/p/19e010b2a4c0)
* [爬取简书全站文章并生成 API（三）](http://www.jianshu.com/p/f30788fddaf2)
* [爬取简书全站文章并生成 API（四）](http://www.jianshu.com/p/9e1d12500f78)
* [爬取简书全站文章并生成 API（五）](http://www.jianshu.com/p/4e4c85e1e2b8)

### 1. 爬取前的准备

了解简书整个网站的结构以及分析网页源代码：


### 2. 爬取简书全站

爬取简书“新上榜”，“热门”中的文章并保存在 MySQL 中。


### 3. 爬取搜索到的文章

本来想爬取简书中某一类技术文章，由于简书没有明显的分类目录，文章也没有对应的 `tag` 所以准备爬取搜索到的文章。


对于搜索的文章只能爬取前 100 页，每页 10 条数据。


### 4. 生成 API

将上面爬取到的文章保存到 **MySQL** 中，使用 **Django REST framework** 来生成 **API**。

![简书 API](http://cdn.tianfeiyu.com/jianshuapi.png)


### 5. 部署上线

* 使用 **nginx + uwsgi + django + supervisor** 进行环境部署

	或者

* 使用 **docker** 进行环境部署



> #### -_- 目前代码写的比较散乱，后面还会不断重构，如有任何建议，欢迎提 issue，欢迎 fork，pr，当然也别忘了 star 哦！

---
