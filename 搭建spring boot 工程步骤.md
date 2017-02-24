## 搭建spring boot 工程步骤
### 1.创建maven工程
```
利用IDEA创建maven-archtype-webapp
```
### 2. 修改pom文件
```
<parent>
    <groupId>org.springframework.boot</groupId>
    <artifactId>spring-boot-starter-parent</artifactId>
    <version>1.4.3.RELEASE</version>
  </parent>
```
```
<dependency>
        <groupId>org.springframework.boot</groupId>
        <artifactId>spring-boot-starter-web</artifactId>
</dependency>
```
### 3.创建启动入口
```
public static void main(String[] args) throws Exception {
        SpringApplication.run(Example.class, args);
}
```
### 4.运行
```
mvn spring-boot:run
```
### 5.创建可执行的jar（fat jar）
```
删除pom文件中的打成war包的文件
```
```
<build>
    <plugins>
        <plugin>
            <groupId>org.springframework.boot</groupId>
            <artifactId>spring-boot-maven-plugin</artifactId>
        </plugin>
    </plugins>
</build>
```

### 6.查看jar文件内容（optional）
```
jar tvf target/micro-service-1.0-SNAPSHOT.jar
```
### 7.运行jar文件
```
java -jar target/micro-service-1.0-SNAPSHOT.jar
```
### 8.访问localhost:8080
