# MdDealWithImg2-Base64OrLocal-、
[GitHub](https://github.com/96bearli/MdDealWithImg2-Base64OrLocal-)
[Blog](https://bear962464.cn/2021/01/25/1088/)
# markdown图片批量处理到本地|base64 or local
写的发GitHub的英文版readme不能浪费是不是
**>_<**
## What's this?
Localization of image links referenced in markdown documents .
 And you have two options: 
 1. Save in Base64 format; 
 2. Reference local images.
 
## 这是个啥？
将markdown文档引用的图片链接本地化
 你有两种选择： 
 1. 保存img为base64格式; 
 2. 引用下载到本地的图片.

ps：不太推荐1，特别是大量图片的文件，更容易出现种种问题，而且文档打开速度，1.2倍的大小等等，这些都是不利条件

## And How to use it?
 * Put the document you want to process in the folder "before".
 * Then run main.py.
 * You can find the new documents in the folder "output".

## 怎么用？
 * 把你想处理的.md文档放在before文件夹中
 * 运行主程序main.py.
 * 输出文件会保存到output文件夹

ps: 两种模式图片都会保存到output内同名文件夹，图片可能会请求失败或404，但是会创建一个空的图片文件顶位置。 

另外每次运行output文件夹**自动重置清空**

## Import

~~~python
import re
import os
import urllib.error
import urllib.request
import shutil
import base64
~~~
