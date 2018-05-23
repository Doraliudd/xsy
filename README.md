# 简介
本文档旨在帮助用户了解销售易eclipse插件功能，快速掌握插件的操作方法。通过应用实例帮助用户快速使用。
# 前提条件
- 开发者必须具备一定的Java研发能力，能够使用Java开发工具进行开发、编译、运行以及调试。
- Eclipse版本要求：neon.2。
- 获取销售易Eclipse插件：Eclipse插件由销售易相关开发人员提供。
- 获取SecretCode：用户授权密码由销售易相关开发人员提供。

[帮助文档](https://crm.xiaoshouyi.com/doc/document/index.html)

```java
package other.ajbckk.bdicfkbfkkfaa;
public class Test {
}
```
![image](https://user-images.githubusercontent.com/24582613/40411769-f0ab8790-5ea3-11e8-8a39-306c43de97d8.png)

![](https://crm.xiaoshouyi.com/doc/document/docs/productDoc/v1804/developerGuide/H5/developerGuide/Responsive HTML5_favicon.png)

[sample](#sample)


沙盒环境与生产环境的物理隔离：

• 沙盒环境与生产环境在物理服务上的隔离：独立的代码运行服务器；独立的数据库服务；独立的网络安全防护等

• 沙盒环境中的文件相关的内容存储也需要独立的环境来进行文件存储服务

• 沙盒环境的运行不会影响生产环境的正常运行



系统性能：

• 沙盒环境的性能可以弱于生产环境，并且沙盒环境上不提供客户做性能测试的能力，以保证资源的可用性

• 沙盒环境所占用的服务器资源，节点数量等资源需要规划一下



访问地址：

• 沙盒环境使用独立的域名进行登录访问，新的域名：https://test.xiaoshouyi.com

• 如果租户开启了 PRM 能力，PRM 访问的域名也会发生变化，新的域名：https://

• 沙盒环境对应的服务端页面代码访问的路径也会发生变化，新的域名：https://

• Open API，Bulk API 访问的 URL 信息也有独立的新的地址：

   https://api-test.xiaoshouyi.com



环境标识区分：

• 沙盒环境在使用过程中也是有别于生产环境，在使用页面上会有明确的标识来区分沙盒环境。

• PC端顶部有沙盒环境标识

• 移动端沙盒环境App的LOGO 与生产环境App不一样, 沙盒中的用户信息中有沙盒环境标识





移动端的沙盒环境：

• 安卓使用独立的沙盒App, iOS会提供TestFlight版的App

网页端的沙盒环境：

• 使用不同的 URL 来访问沙盒环境的 Web 端

• 其他的主体逻辑与现有的相同




# sample
什么是沙盒环境？

• 沙盒环境是一个从生产环境复制所有的配置数据，在物理上与生产环境隔离，使用独立的有别于生产环境的登录地址，用户客户的新功能的开发，测试，培训的一套独立的租户环境。

• 沙盒环境上的任何操作不会影响生产环境上的操作。





沙盒环境的分类：

• 开发者版本：

  • 复制所有生产环境的配置数据，但不包含业务数据



• 部分复制版本：

  • 复制所有生产环境的配置信息，并包含部分的业务数据

  • 业务数据的范围是由用户自己定义的，但是需要用户创建对应的模板



• 完整版本：

  • 复制所有生产环境的配置信息

  • 复制所有生产环境的业务数据，这里的业务数据主要包含 CRM 中的业务数据，协同办公相关的数据不复制，比如日程相关的数据；费用审批单相关的数据；以及社交相关的数据，比如工作圈内容，聊天记录等
