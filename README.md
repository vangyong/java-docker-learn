# docker测试工程-java

# maven环境
setting.xml

<pluginGroups>  
    <pluginGroup>com.spotify</pluginGroup>  
</pluginGroups>

<server>
  <id>docker-registry</id>
  <username>vangyong</username>
  <password>*****</password>
  <configuration>
      <email>vangyong@126.com</email>
  </configuration>
</server>

# 项目工程中添加
docker-registry

# 构建
* 构建
mvn package docker:build
* 构建并push到仓库
mvn clean package docker:build -DpushImage 


