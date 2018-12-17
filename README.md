# MSRecordManager
基于TAAE([The Amazing Audio Engine](https://github.com/TheAmazingAudioEngine/TheAmazingAudioEngine))框架封装的录音工具类 可以直接添加到项目中使用

在开始之前,先通过一张图简单的总结一下 iOS当中常用的音频框架

![iOS音频框架](https://github.com/scyios/MSRecordManager/blob/master/img/image1.png)

每个类的详细说明在请参照[这里](https://objccn.io/issue-24-4/)或[官方文档](https://link.jianshu.com/?t=https://developer.apple.com/library/ios/documentation/AudioVideo/Conceptual/MultimediaPG/UsingAudio/UsingAudio.html#//apple_ref/doc/uid/TP40009767-CH2-SW6);我不多做赘述, 在这提两点

1) iOS中所有的音频技术都构建在 Audio Unit 这个框架之上
2) TAAE 主要是封装了Audio Unit、AudioToolBox、AVFoundation

## 工作流程
由于我的项目录音模块没有涉及到音效混合,所以业务逻辑还算是比较简单,还是用一张图来描述
![iOS音频业务逻辑](https://github.com/scyios/MSRecordManager/blob/master/img/image2.png)
