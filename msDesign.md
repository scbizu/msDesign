## 《微服务设计》中提到的书籍 && 工具

--------------

### 数据备份

* [Aegisthus](https://github.com/Netflix/aegisthus)：Netflix的处理大量数据的流水线


### 部署

* [Packer](http://www.packer.io/): 跨平台生成镜像工具

* 虚拟化服务

  * hypervisor
  * Vagrant
  * Docker


* [Kubernetes](https://kubernetes.io/): Docker集群管理
* [Deis](https://deis.com/) :基于Docker(k8s)的类似[Heroku](https://www.heroku.com/)的PaaS

* 《持续交付》

* [Terraform](https://www.terraform.io/)  管理部署可预测的生产环境

### 测试

*  《敏捷软件测试》
*  《Scrum 敏捷软件开发》
* 《测试驱动的面相对象软件开发》 Mock还是打桩测试？

* [Mountbank](http://www.mbtest.org) 打桩mock服务器

### 监控

* [Nagios](https://www.nagios.org/) 监控服务
* [ssh-multiplexers](http://omnitty.sourceforge.net/) 在不同主机运行相同命令
* [logstash](http://logstash.net) 专门的日志收集工具 可以解析多种不同的日志格式
* [Kibana](https://www.elastic.co/products/kibana) 基于es(elasticsearch)的查看日志的系统
* [Graphite](https://graphiteapp.org/)  API日志指标聚合  可以单样本聚合 也可以跨样本聚合
* [Metrics](http://metrics.codahale.com/) 运行在JVM上的库 用来存储指标 例如 计数器/计时器/计量表
* [Zipkin](https://twitter.github.io/zipkin) 提供详细的服务间调用的跟踪信息。
* 《Information Dashboard Design:Displaying Data for AtaGlance Monitoring》 图形化监控
* [Riemann](http://riemann.io/) 一个事件服务器 允许高级的事件聚合和事件路由
* [Suro](https://github.com/Netflix/suro) Netflix的数据流水线 处理用户行为相关的指标 和 运营数据。

### 安全

* SSO(单点登录)
  * [SAML](http://saml.xml.org/)
  * [OpenID Connect](http://openid.net/connect/)
* [ModSecurity](https://modsecurity.org/) 应用程序防火墙 在特定的IP范围限制连接数 并检测其他类型的恶意攻击
* iptables
* [SCCM](https://www.microsoft.com/en-us/cloud-platform/system-center-configuration-manager) Windows补丁/软件管理
* [Spacewalk](http://spacewalk.redhat.com/) Linux(Fedora,CentOS Scientific Linux)软件管理
* [Ansible](https://www.ansible.com/) DevOps工具
* [Puppet](https://puppet.com/) DevOps工具
* [Chef](https://www.chef.io/) DevOps工具
* [AppArmor](http://wiki.apparmor.net/index.php/Main_Page) 易用的Linux APP 安全管理系统（Ubuntu && SuSE）
* [SeLinux](https://fedoraproject.org/wiki/SELinux)  (RedHat)
* [GrSSecurity](https://grsecurity.net/) 对Linux Kerner的安全增强

### 微服务规模化

* 《REST实战》(但是据说翻译不太好  可以看《RESTful WEB APIs》)
* [Zookeeper](http://zookeeper.apache.org/)  配置管理  服务间的数据同步 leader选举 消息队列和命名服务
* [Consul](http://www.consul.io/) 支持配置管理 和 服务发现 **提供了现成的DNS服务器实现** 支持HTTP的REST API
* [Eureka](http://github.com/Netflix/eureka)  相比以上两者 优点是提供了 **负载均衡的实现** 支持REST API
* [Swagger](http://swagger.io/) API文档完善
* [HAL和HAL浏览器](http://stateless.co/hal_specification.html) **超媒体控制** HAL浏览器可以让用户在线调用我们的API
* 再一次提到了《Release it!》
