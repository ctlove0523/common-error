## 编译告警

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

## 执行findbugs检查失败

[ERROR] Failed to execute goal org.codehaus.mojo:findbugs-maven-plugin:3.0.3:findbugs (default-cli) on project iobm: Unable to parse configuration of mojo org.codehaus.mojo:findbugs-ma
ven-plugin:3.0.3:findbugs for parameter pluginArtifacts: Cannot assign configuration entry 'pluginArtifacts' with value '${plugin.artifacts}' of type java.util.Collections.Unmodifiable
RandomAccessList to property of type java.util.ArrayList -> [Help 1]

解决方法：升级插件版本到3.0.4
