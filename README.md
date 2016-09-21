# imoocDownloader
[![Build Status](https://travis-ci.org/webbought/imoocDownloader.svg?branch=v1.1.0)](https://travis-ci.org/webbought/imoocDownloader)    [![codecov](https://codecov.io/gh/webbought/imoocDownloader/branch/v1.1.0/graph/badge.svg)](https://codecov.io/gh/webbought/imoocDownloader)

###简介

imoocDownloader 用来爬取慕课网上指定课程id视频


###安装

```shell
git clone https://github.com/webbought/imoocDownloader.git

cd imoocDownloader 

npm install
```



###Usage
```javascript
'use strict'

module.exports = {
    rootDir : __dirname,
    timeout : 10,
    videoDir : './video',
    target : [552,556,21,441,11]
}
```

#####配置好config文件，执行 `node index.js`即可。 
 
###指令模式
```shell
node index.js <command> <arguments>
```

*    command
    *    --search 查找 后面必须有所要查找的关键词参数
        *    arguments {String} search word
    *    --list 课程列表  后面必须有所要查看的课程ID
        *    arguments {Number} course id
    *    --download 下载  后面必须有所要下载的课程ID
        *    arguments {Number} course id
    
####example
```shell
node index.js --search node
```
![search][1]

```shell
node index.js --list 434
```
![list][2]

```shell
node index.js --download 434
```
![download][3]
```
课程目录
```
![course][4]
```
章节目录
```
![chapter][5]
```
视频目录
```
![video][6]


[1]: https://github.com/webbought/imoocDownloader/blob/master/img/1.png "search"
[2]: https://github.com/webbought/imoocDownloader/blob/master/img/2.png "list"
[3]: https://github.com/webbought/imoocDownloader/blob/master/img/3.png "download"
[4]: https://github.com/webbought/imoocDownloader/blob/master/img/4.png "course"
[5]: https://github.com/webbought/imoocDownloader/blob/master/img/5.png "chapter"
[6]: https://github.com/webbought/imoocDownloader/blob/master/img/6.png "video"