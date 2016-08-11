#spring-boot-web-template
1）该项目可作为spring boot开发web项目时使用的模板

2）在build.gradle文件中引入了对于spring web, spring data jpa, spring data redis, mysql等基础依赖，可以满足基本web和访问数据库的需求。

3）因为在gradle中引入了data jpa 和 mysql 依赖，相应地，必须要在application.properties中加入spring.jpa和spring.datasource的相关配置项，否则运行会出错。

4）从该项目拷贝后新建其他项目时，除了使用Eclipse refactor功能修改包名和类名之外，还需要记得做一次“gradle task: clean”，清除该模板项目的构建残留信息，否则，直接运行“gradle task: bootRun”，会提示出错。