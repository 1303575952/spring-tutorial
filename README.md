<p align="center">
    <a href="https://spring.io/projects/spring-framework" target="_blank" rel="noopener noreferrer">
        <img src="http://dunwu.test.upcdn.net/common/logo/spring.png" alt="spring-logo">
    </a>
</p>

<p align="center">
    <a href="https://creativecommons.org/licenses/by-sa/4.0/" target="_blank" rel="noopener noreferrer">
        <img src="https://badgen.net/github/license/dunwu/spring-tutorial">
    </a>
    <img alt="Spring Boot Version" src="https://img.shields.io/badge/spring-5.0.2.RELEASE-blue">
    <img src="https://img.shields.io/badge/maven-v3.6.0-blue" alt="maven">
    <img alt="Build" src="https://api.travis-ci.com/dunwu/spring-tutorial.svg?branch=master">
</p>

<h1 align="center">Spring Tutorial</h1>

> **`spring-tutorial`** 是一个以简单范例来展示 spring 在 web 开发中的各种应用的教程。
>
> - 🔁 项目同步维护：[Github](https://github.com/dunwu/spring-tutorial/) | [Gitee](https://gitee.com/turnon/spring-tutorial/)
> - 📖 电子书阅读：[Github Pages](https://dunwu.github.io/spring-tutorial/) | [Gitee Pages](http://turnon.gitee.io/spring-tutorial/)

## 文档

> 📖 [**spring-tutorial 文档在线阅读**](https://dunwu.github.io/spring-tutorial/)
>
> 扩展学习：
>
> - [Java 教程](https://github.com/dunwu/java-tutorial)
>   - [JavaCore 教程](https://dunwu.github.io/javacore/)
>   - [JavaWeb 教程](https://dunwu.github.io/javaweb/)
>   - [Spring Boot 教程](https://dunwu.github.io/spring-boot-tutorial/)

|       0️⃣       |       1️⃣       |       2️⃣       |      3️⃣      |       4️⃣       |       5️⃣       |
| :-----------: | :-----------: | :-----------: | :---------: | :-----------: | :-----------: |
| [综合](#综合) | [核心](#核心) | [数据](#数据) | [Web](#Web) | [集成](#集成) | [安全](#安全) |

### 综合

- [Spring 面经](docs/summary/spring-interview.md)
- [Spring 概述](docs/summary/spring-overview.md)

### 核心

> [核心](docs/core/README.md) 章节主要针对：Spring 框架的核心技术。如；IOC 依赖注入、AOP、数据绑定等。

- [Spring IoC](docs/core/ioc.md)
- [Spring AOP](docs/core/aop.md)
- [Spring Resources](docs/core/spring-and-resources.md)

### 数据

> [数据](docs/data/README.md) 章节主要针对：Spring 在数据库领域的应用。如：JDBC、ORM、事务等。

- [Spring 的数据访问策略](docs/data/data-access-in-spring.md)
- [Spring 中使用 JDBC 访问数据](docs/data/spring-and-jdbc.md)
- [事务管理](docs/data/transaction.md)

### Web

> [Web](docs/web/README.md) 章节主要针对：Spring 在 web 领域的应用。如：Spring MVC、WebSocket 等。

- [SpringMVC 简介](docs/web/spring-mvc.md)

### 集成

> [集成](docs/integration/README.md) 章节主要针对：Spring 与第三方框架、库集成。如：Cache、Scheduling、JMS、JMX 等。

- [Spring 集成 Dubbo](docs/integration/spring-and-dubbo.md)
- [Spring 集成缓存](docs/integration/spring-and-cache.md)
- [Spring 集成调度器](docs/integration/spring-and-scheduler.md)

### 其他

- [spring 4 升级踩雷指南](docs/others/spring4-upgrade.md)
- [资源](docs/others/resources.md)

## 示例

### 说明

#### 重要库版本

| 库或工具             | 版本            | 说明                                                         |
| -------------------- | --------------- | ------------------------------------------------------------ |
| Spring Framework     | 5.0.2.RELEASE   |                                                              |
| JDK                  | 1.8+            | Spring5 开始，要求 JDK8+                                     |
| Maven                | 3.5.2           | 本项目使用 [maven](https://maven.apache.org/index.html) 作为构建工具。 |
| jetty-maven-plugin   | 9.4.8.v20171121 | [Jetty](http://www.eclipse.org/jetty/) 可作为 web 服务器和 servlet 容器。此插件可以免部署启动 web app。 |
| tomcat7-maven-plugin | 2.2             | [Tomcat](https://tomcat.apache.org/index.html) 可作为 web 服务器和 servlet 容器。此插件可以免部署启动 web app。Tomcat 早已经发布 Tomcat8，但是 maven 插件 一直没有提供 tomcat8 的支持（最后更新为 2013 年）。 |

#### 启动

为了便于展示示例，所有 war 包形式的项目都可以使用 maven 插件快速启动嵌入式服务器，支持 Tomcat 和 Jetty 两种方式。

Tomcat7 嵌入式服务器启动：

```bash
$ mvn tomcat7:run -Dmaven.test.skip=true
```

Jetty 嵌入式服务器启动：

```bash
$ mvn jetty:run -Dmaven.test.skip=true
```

如果子项目中无特殊说明，默认端口配置为 8089，当然，你可以自己指定。

启动成功后，访问 http://localhost:8089 。

#### 规范

- 推荐使用 [IDEA](https://www.jetbrains.com/idea/) 作为 IDE
- 代码规范使用 [阿里巴巴 Java 开发手册](https://github.com/alibaba/p3c)
  - 如果你使用 IDEA 作为你的 IDE，推荐安装 Alibaba-Java-Coding-Guidelines 插件来做静态检查。

## License

本博客所有文章除特别声明外，均采用 [![License: CC BY-NC-SA 4.0](https://licensebuttons.net/l/by-nc-sa/4.0/80x15.png)](https://creativecommons.org/licenses/by-nc-sa/4.0/) 许可协议。
