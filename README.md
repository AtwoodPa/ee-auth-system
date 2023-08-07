# ee-auth-system

本文档提供了关于实现Spring Boot + Vue通用权限管理系统的技术说明和使用指南。
我们将使用以下技术栈进行开发：

- 前端：Vue全家桶、Element-Plus
- 后端：Spring Boot、Spring MVC 5.x、MyBatis Plus、Spring Security + JWT、SSM、Redis

## 前端技术栈

### Vue全家桶

Vue全家桶是指Vue.js框架的一组相关库，包括Vue核心库、Vue Router和Vuex。Vue核心库用于构建用户界面，Vue Router用于处理路由导航，Vuex用于状态管理。通过使用Vue全家桶，我们可以更高效地开发和管理前端代码。

### Element-Plus

Element-Plus是一套基于Vue.js的UI组件库，提供了丰富的UI组件和样式。我们可以使用Element-Plus来构建用户界面，使其具有美观和易用的特点。

## 后端技术栈

### Spring Boot

Spring Boot是一个用于开发Java应用程序的框架，它简化了Spring应用程序的配置和部署过程。我们将使用Spring Boot来构建后端服务。

### Spring MVC 5.x

Spring MVC是一个基于Java的Web框架，用于构建Web应用程序。我们将使用Spring MVC 5.x来处理HTTP请求和构建RESTful API。

### MyBatis Plus

MyBatis Plus是一个基于MyBatis的ORM框架，提供了更简单和便捷的数据库操作方式。我们可以使用MyBatis Plus来与数据库进行交互，实现数据的增删改查操作。

### Spring Security + JWT

Spring Security是一个用于身份验证和授权的框架，可以帮助我们保护后端API的安全性。我们将结合JWT（JSON Web Token）来实现基于Token的身份验证和授权机制，确保只有经过认证的用户才能访问受保护的API。

### SSM

SSM是指SpringMVC、Spring和MyBatis的组合，是一种常用的Java Web开发框架。我们将使用SSM框架来构建后端的业务逻辑和数据访问层。

### Redis

Redis是一个高性能的键值存储数据库，我们将使用Redis来缓存用户会话和权限信息，提高系统的性能和扩展性。

## 开发环境要求

在开始使用Spring Boot + Vue通用权限管理系统之前，请确保你的开发环境满足以下要求：

- JDK：建议使用JDK 1.8.x或更高版本。
- MySQL：建议使用MySQL 8.0.x或更高版本作为数据库。
- Maven：建议使用Maven 3.5.x或更高版本作为项目构建工具。
- 数据库连接池：我们将使用Druid 1.x作为数据库连接池。
- 日志管理：我们将使用SLF4J和Log4j来进行日志管理。

## 使用指南

以下是使用Spring Boot + Vue通用权限管理系统的一般步骤：

1. 克隆项目代码：使用Git工具克隆该系统的代码到本地开发环境。

2. 后端开发：进入后端项目目录，根据实际需求配置数据库连接和其他相关配置。然后，使用命令行工具运行`mvn spring-boot:run`命令启动后端服务，开始编写和调试后端代码。

3. 前端开发：进入前端项目目录，使用命令行工具运行`npm install`安装项目依赖。然后，使用`npm run dev`命令启动开发服务器，开始编写和调试前端代码。

4. 数据库准备：根据项目要求，创建数据库并导入相应的表结构。可以使用MyBatis Plus提供的代码生成工具来生成数据库表对应的实体类和Mapper接口。

5. 接口对接：在前端代码中，根据后端提供的API文档，使用HttpClient或其他方式与后端进行接口对接，获取和提交数据。

6. 测试和调试：在开发过程中，进行测试和调试，确保前后端的交互和功能正常。

7. 构建和部署：完成开发后，使用前端工具构建前端代码，并将其部署到Web服务器上。同时，将后端代码打包成可执行的JAR文件，并部署到服务器上。确保正确配置Redis服务器，并在系统中使用Redis缓存用户会话和权限信息。



