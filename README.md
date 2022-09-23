# Musicer
旨在将网易云、酷狗、QQ、酷我等各音乐平台集于一体

## 项目概述

<div align=center>
	<img src="imgs/vip.png"/>
</div>

&emsp;&emsp;各大音乐平台是从何时开始收费的这个问题没有追溯过，印象中酷狗在16年就已经开始收费了，貌似当时的收费标准是付费音乐下载一首2元，会员一月8元，可以下载300首。虽然下载收费，但是还可以正常听歌。陆陆续续，各平台不仅收费，而且还更在乎版权问题，因为缺少版权，酷狗上以前收藏的音乐也不能听了，更过分的是，有些歌非VIP会员只能试听60秒(•́へ•́╬)。

&emsp;&emsp;版权问题重视起来当然是好事，但只是闲暇时来听听音乐放松一下自己的我来说，不会因为想听音乐而开通各个音乐平台的VIP的┗( ▔, ▔ )┛，所以渐渐就有了些想法：能不能将这些音乐整合起来，比如我去酷狗音乐听某一首歌，发现没有版权或只能试听，能不能自动去网易云音乐搜索下载到本地(干脆直接下载到酷狗对应的文件夹里)，如果还没有就去QQ音乐、虾米音乐、百度音乐等等。

&emsp;&emsp;本项目就是在这样的背景下，通过对各音乐平台进行逆向分析，然后enmmmmm，可以听到自己喜欢的歌曲......由于各音乐平台网站会不定期进行维护，导致爬虫代码也需要进行相应地更新，为了方便维护本项目，于是将其开源(≧∀≦)♪

&emsp;&emsp;**警告！！！本项目所涉及的内容仅供学习、交流，请勿将其用于非法用途！！！**

<div align=center>
	<img src="imgs/warning.png"/>
</div>

## 食用方式
```
# 先安装环境所需的依赖包
pip install -r requirements.txt
```
```
# 运行项目
python main.py
```
## 运行效果如下:
```
D:\ProgramData\Anaconda3\envs\Spider\python.exe E:/Program/Python/Spider/Musicer/main.py

        ###   ###       ###     ###     ######    ######     ######   ########   ####### 
       ## ## ## ##      ###     ###   ###           ##     ###        ###        ##   ### 
      ##   ###   ##     ###     ###     ######      ##     ##         ########   ####### 
     ##    ###    ##    ###########         ###     ##     ###        ###        ##  ##  
    ##             ##   ###########     ######    #######   #######   ########   ##   ####

目前支持的播放器类型: 1. 网易云	2. 酷狗	3. 酷我
请选择播放器类型(-1退出): 1
请输入歌名或歌手: 本兮
*************************************搜索结果如下*************************************
序号　　　歌名　　　　　　　　　　　　　　　　　　歌手　　　　　　　　时长(s)　　　　　专辑　　　　　　　　　　　　　　　　　　
------------------------------------------------------------------------------------
0　　　　情花　　　　　　　　　　　　　　　　　　本兮　　　　　　　　239　　　　　　　本兮　　　　　　　　　　　　　　　　　　
1　　　　一个深爱的女孩　　　　　　　　　　　　　本兮　　　　　　　　230　　　　　　　热门华语271　　　　　　　　　　　　　
2　　　　你在看孤独的风景（翻自 本兮（马晓晨）））忆迟　　　　　　　　250　　　　　　　你在看孤独的风景　　　　　　　　　　　　
3　　　　客官不可以　　　　　　　　　　　　　　　本兮　　　　　　　　102　　　　　　　最美的光　　　　　　　　　　　　　　　　
4　　　　纪念　　　　　　　　　　　　　　　　　　本兮　　　　　　　　240　　　　　　　本兮　　　　　　　　　　　　　　　　　　
5　　　　一直在等　　　　　　　　　　　　　　　　本兮　　　　　　　　253　　　　　　　一直在等　　　　　　　　　　　　　　　　
6　　　　坏女孩　　　　　　　　　　　　　　　　　本兮　　　　　　　　244　　　　　　　洛芸汐的翻唱　　　　　　　　　　　　　　
7　　　　创作者　　　　　　　　　　　　　　　　　徐良　　　　　　　　248　　　　　　　创作者　　　　　　　　　　　　　　　　　
*************************************************************************************
请输入要下载歌曲的序号(-1退出): 0
下载完毕!
请输入要下载歌曲的序号(-1退出): -1

Process finished with exit code 0
```

## 更新记录
- 2020/10/24 项目开源，实现了网易云付费音乐、酷狗音乐爬取
- 2021/04/23 对酷狗音乐API做了部分修改，为方便后面的集成，对项目框架做了一些改动
- 2021/05/17 添加了对酷我音乐的爬取，并支持音乐品质的选择，包括流畅音质、高品音质和超品音质
- 2022/08/31 
  * 支持对网易云音乐音质的选择，添加歌词API和专辑图片API
  * 更新酷狗音乐解析参数，添加歌词API和专辑图片API
  * 更新酷我音乐解析参数

## 我的博客
- 我在CSDN开设的有相应的系列专栏，里面有详细地分析过程，可以参考哦！**如果您觉得本项目对您的学习有所帮助，记得在右上角点个Star哦φ(≧ω≦\*)♪**

- 我的[爬虫系列专栏地址](https://blog.csdn.net/qq_42730750/category_10252266.html): https://blog.csdn.net/qq_42730750/category_10252266.html

- 我的[博客地址](https://blog.csdn.net/qq_42730750): https://blog.csdn.net/qq_42730750

## 联系我
- 邮箱：youran.xia@foxmail.com
