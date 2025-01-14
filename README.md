# SaveMyGame

一个即时文件保存工具。用于定时自动保存某文件夹的文件，并提供还原点可以一键还原。

对于一命通关或者硬核游戏等不支持存档备份和还原点的游戏极为有用。

<img src="README.assets/image-20240312095437997.png" alt="image-20240312095437997" style="zoom:50%;" />

## 已经实现的功能

* 支持选择文件夹，自动打包压缩到指定文件夹进行备份
  * 允许选择压缩等级（简易）
  * 允许使用仅存储压缩等级

* 支持一键还原打包的备份文件到源文件夹

* 支持定时自动备份。
* 支持按照时间顺序自动删除旧文件防止备份文件过大，默认将保留最新的10个文件
  * 目标文件夹过大时会提示

* 应用程序自动恢复上一次配置，并且存储存档位置、存档恢复位置等属性。
* ~~i18n支持~~
  * 未来可能会支持

## TODO

* 使用FileSystemWatcher替代轮询

## 构建和安装

使用下述指令发布（项目中已经包括了一个默认的发布选项）：

```
dotnet publish
```

使用PublishSingleFile+win-x86生成文件体积为15M

