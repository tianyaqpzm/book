

# X-GEN

## 1、项目背景

项目中存在很多重复的基础功能：CURD 、翻页

因此 减少重复，聚集挑战的部分

在基础之上 进行业务开发

面临问题： 

* 生成的配置文件发生变化，那么读取配置文件的程序需要变化

* 模版文件发生变化
* 调用逻辑和调用顺序变化
* 输出格式变化

X-GEN 将生成应用的核心部分独立， 公共应用+ 自定义模版

 按照模版和配置文件，生成结果的通用框架，支持模版自定义，支持配置方式自定义、支持生成方式自定义，深圳自定义生成的过程。

解决：

根据什么生成，如何生成， 生成利用外部主题，生成格式，以及生成地方

## 2、 功能概述

- 配置管理geninvocation:  获取用户配置，缓存配置，并对外提供接口
- 分发调度模块 dispatch: 只负责接受用户任务，组合任务，然后分发任务，只起到调度的作用，本身不处理用户的请求
- 生成代理功能:

* 模版管理

* 生成输出
