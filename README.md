<div>
<h1 align="center">欢迎使用 TJMU-Teacher-Evaluation 👋</h1>
</div>

![python_vesion](https://img.shields.io/badge/Python-3.5%2B-green.svg)![GitHub stars](https://img.shields.io/github/stars/L1cardo/TJMU-Teacher-Evaluation.svg?style=social)![Twitter Follow](https://img.shields.io/twitter/follow/AlbertAbdilim.svg?label=Follow&style=social)
[![weibo](https://img.shields.io/badge/微博-@ABD_R3yiM-red.svg)](https://www.weibo.com/ABD_R3yiM)

> 华中科技大学同济医学院教师评教脚本

## 声明

本项目改自[liuyi12138](https://github.com/liuyi12138/HustPingJiao)大佬的项目，再次感谢大佬的制作。主校区的同学移步至大佬的[项目](https://github.com/liuyi12138/HustPingJiao)

liuyi12138制作的是适用于主校区的情况，只适用于一门科目只有一个待评价老师的情况。但是在同济校区这边，一门课往往由多名老师（最高36个老师,所有科目加起来上百个老师，无力吐槽）授课，所以就不太好用。

我自己修改了一些代码，对于同济的学生会好用一些

## 🏠 [主页](https://github.com/L1cardo/TJMU-Teacher-Evaluation)

## 说明

本人算是程序爱好者，目前没有达到真的是“一键”脚本，还是有些需要手动的情况

目前只能完成评教页面第一页的所有科目的评教，第二页的url获取还是没搞清楚

一次只能评教所有科目的第一个老师，第二个老师还是需要修改参数重新运行

## 安装

1. 首先你得要有python3，并且安装 selenium，安装命令为

```python
  pip3 install selenium
```

2. 要有 Chrome 浏览器（必须是Chrome本身，不能是其他Chrome内核的浏览器）

3. 下载 chromedriver 
   
   可以在[这里](http://npm.taobao.org/mirrors/chromedriver/)下载你的电脑系统对应的版本
   
   ① Windows 用户下载以后，新建一个命名为 hromedriver 的文件夹，将解压的 chromedriver.exe放进文件夹，再配置进path环境变量 
   
   ② Mac 用户强烈推荐使用 Homebrew 安装(你得要自己安装 Homebrew），Homebrew 下安装命令为
   
   ```bash
   brew install chromedriver
   ```
   
   ③ Linux用户，把下载好的文件放在 /usr/bin 目录下就可以了

## 配置

打开 evaluation.py 文件，修改第7、8、9行的三个参数，如下

```
ACCOUNT = " " #填写学号
PASSWORD = " " #填写统一认证平台密码
TEACHER = 1 #要评价某一科目的第几个老师,最小值为 1
```

## 运行

在文件夹根目录运行下面的命令 

```python
python3 evaluation.py
```

运行结束后，网页会停止，此时已经评教完第一页所有科目的第一个老师，此时修改上面的 `TEACHER = 1` 为 `TEACHER = 2` 后再运行，以此类推直至第一页的所有老师全部评教完

## 作者

👤 **Albert**

* Twitter: [@AlbertAbdilim](https://twitter.com/AlbertAbdilim)
* Github: [@L1cardo](https://github.com/L1cardo)
* 微博:[@ABD_R3yiM](https://www.weibo.com/1935602951)

## 🤝 贡献

欢迎做出贡献，提出问题以及提出建议!

请查看 [issues](https://github.com/L1cardo/TJMU-Teacher-Evaluation/issues) 页面.

## 希望支持

如果这个项目帮助到你的话，一个Star ⭐️！

如果你想更进一步支持的话，可以适当地进行[打赏](https://raw.githubusercontent.com/L1cardo/images/master/TJMU-Teacher-Evaluation/alipay.jpg)
