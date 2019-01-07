### 不用编译安装

0. 不用编译，直接使用是在centos 7.5上编译的

1. use-directly文件夹下为不用编译直接使用的,必须解压到/usr/local目录

       tar -xf sqlparser.tar.gz -C /usr/local
       chmod +x sqladvisor
       mv sqladvisor /usr/bin/sqladvisor


2. echo "你的慢日志"| sqladvisor  或者

       sqladvisor -h 127.0.0.1 -P 3306 -u root -p 123456 -d test -q "select version();"



### 一、简介

SQLAdvisor是由美团点评公司技术工程部DBA团队（北京）开发维护的一个分析SQL给出索引优化建议的工具。它基于MySQL原生态词法解析，结合分析SQL中的where条件、聚合条件、多表Join关系 给出索引优化建议。**目前SQLAdvisor在美团点评内部广泛应用，公司内部对SQLAdvisor的开发全面转到github上，开源和内部使用保持一致**。
    
**主要功能：输出SQL索引优化建议**

### 二、SQLAdvisor详细说明

1. [SQLAdvisor快速入门教程](./doc/QUICK_START.md)
2. [SQLAdvisor架构和实践](./doc/THEORY_PRACTICES.md)
3. [SQLAdvisor release notes](./doc/RELEASE_NOTES.md)
4. [SQLAdvisor开发规范](./doc/DEVELOPMENT_NORM.md)
5. [FAQ](./doc/FAQ.md)

### 三、SQLAdvisor的需求及Bug反馈方式

如果用户在实际的应用场景中对SQLAdvisor有新的功能需求，或者在使用SQLAdvisor的过程中发现了bug，在github上进行交流或是PullRequest，也可以在讨论组/群进行反馈，我们会及时维护。

![QQ](./doc/img/qq.png)


