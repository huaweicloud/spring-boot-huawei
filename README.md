[![Build Status](https://github.com/huaweicloud/spring-boot-huawei/actions/workflows/maven.yml/badge.svg)](https://github.com/huaweicloud/spring-boot-huawei/actions/workflows/maven.yml)
[![License](https://img.shields.io/badge/license-Apache%202-4EB1BA.svg)](https://www.apache.org/licenses/LICENSE-2.0.html)
[![Maven Central](https://maven-badges.herokuapp.com/maven-central/com.huaweicloud/spring-boot-huawei/badge.svg)](https://search.maven.org/search?q=g:com.huaweicloud.devspore%20AND%20a:spring-boot-huawei-dependencies) 

# 介绍
本项目旨在简化基于spring-boot的项目开发时，对于开发环境依赖jar包的管理问题。

## 如何使用
### 基本结构说明
spring-boot-huawei内部模块及简介如下所示:

```$xslt
spring-boot-huawei
 |
 |-spring-boot-huawei-dependencies # 该模块为内部模块的依赖模块，主要功能是提供依赖包的版本管理，其他模块的父模块均直接或间接使用此模块，如无特殊，spring-boot-huawei使用统一版本的jar包。
 |
 |-spring-boot-huawei-parent # 该模块以dependencies模块为父模块，使用其提供的依赖版本管理,本身提供一些插件定义及插件版本管理，作为本项目中其他模块的父模块使用
 |
 |-spring-boot-starter-huawei # 核心组件,该组件提供一个基于spring-boot的web项目最基本的起步依赖
```

### 如何引入依赖
当前只有spring-boot-starter-huawei模块下的各个模块为提供功能起始依赖模块，使用时直接在项目的pom中添加对应版本的功能模块即可，以核心模块为例，使用如下：
```xml
<dependencies>
    <dependency>
        <groupId>com.huaweicloud.devspore</groupId>
        <artifactId>spring-boot-starter-huawei</artifactId>
        <version>${version}</version>
    </dependency>
</dependencies>
```

其他模块参见各模块的文档说明.  
#### 注: 当前各功能模块使用的spring-boot版本为2.5.4，请不要使用过低的spring-boot版本(spring boot 2.0以上)
