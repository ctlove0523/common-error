# 编译告警

**1、[错误信息]** 无法找到类型 'org.junit.jupiter.api.extension.ExtendWith' 的注释方法 'value()': 找不到org.junit.jupiter.api.extension.ExtendWith的类文件

**[解决方法]**
在pom中引入`junit-jupiter-api`
~~~
<dependency>
	<groupId>org.junit.jupiter</groupId>
	<artifactId>junit-jupiter-api</artifactId>
	<version>5.5.2</version>
	<scope>test</scope>
</dependency>
~~~
