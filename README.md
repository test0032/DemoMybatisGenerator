# DemoMybatisGenerator
mybatis自动生成代码简单搭建Demo

### 使用的mybatis的版本
    8.0.17
### 配置步骤
 * 参考文件 generatorConfig.xml
 * 参考文件 pom.xml
    
        <!--mybatis代码生成-->
        <dependency>
            <groupId>org.mybatis.generator</groupId>
            <artifactId>mybatis-generator-core</artifactId>
            <version>1.3.6</version>
        </dependency>
       
        <!--mybatis_generator代码生成器专用  ydx-->
        <plugins>
        <plugin>
            <groupId>org.mybatis.generator</groupId>
            <artifactId>mybatis-generator-maven-plugin</artifactId>
            <version>1.3.6</version>
            <configuration>
                <verbose>true</verbose>
                <overwrite>true</overwrite>
            </configuration>
        </plugin>
        </plugins>
  
 ### 注意事项
    mybatis 8 版本需要注意 
    connectionURL="jdbc:mysql://localhost:3306/springbootdb?useUnicode=true&amp;characterEncoding=utf8&amp;serverTimezone=UTC"
    <classPathEntry location="mysql-connector-java-8.0.18.jar">
