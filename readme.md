# README

## 简介

    本项目是字符串令牌流分割库；

## 功能

字符串令牌解析；
支持令牌流；
解析器可以是自定义字典机械分割，每个token一个独立字典；
解析器也可以是正则表达式；
分割分正向和反向，都是从头开始；
生成对应令牌名称和解析出来的字符创元组，最后剩下的归为一组；

应用场景：各种名称的解析，如中文机构名、药瓶名称标注、地址  =》 加一些地址数据做测试
参考re.scanner

可以用生成器yield来实现；
程序返回元组列表；

## 模块开发

    模块打包    python setup.py sdist
    模块构建    python setup.py build
    模块安装    python setup.py install -e
    模块卸载    手动删除 del D:\Anaconda3\envs\ner\lib\site-packages\neseg

## 附录 - 源码文件说明

    neseg
        /lib
            FMM.py  正向切词
            RMM.py  反向切词
        seg.py      
        main.py   主程序：无界面,参数命令行
    changelog.md    软件更新日志
    readme.md       软件使用、安装指南