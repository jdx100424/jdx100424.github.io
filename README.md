# jdx100424.github.io
jdx test blob


maven配置依赖仓库
在profiles标记上增加
<profile>
      <id>jdk-1.8</id>

      <activation>
        <jdk>1.8</jdk>
      </activation>

      <repositories>
        <repository>
                <id>my-repo</id>
                 <name>my repository</name>
                 <url>http://maven.lifesense.com/nexus/content/repositories/snapshots</url>
                 <releases>
                        <enabled>true</enabled>

                 </releases>
                 <snapshots>
                        <enabled>true</enabled>
                </snapshots>
        </repository>

        <repository>
                <id>my-repo2</id>
                 <name>my repository</name>
                 <url>http://maven.lifesense.com/nexus/content/repositories/releases</url>
                 <releases>
                        <enabled>true</enabled>
                 </releases>
                 <snapshots>
                        <enabled>true</enabled>
                </snapshots>
        </repository>
      </repositories>

    </profile>
