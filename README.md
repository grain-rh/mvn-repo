# mvn-repo

Custom maven artifacts, public repo

# Checkout repo

git clone git@github.com:rewattpower/mvn-repo.git

# Creating a modified 3rd party jar

1. Fork a repo (eg objectify)
2. Clone it
3. Make changes
4. Commit and push changes
5. Make a PR, ideally

# Publishing your jar to Rewatt Maven Repository

1. mvn package
2. mvn install:install-file -Dfile=target/objectify-6.1-SNAPSHOT.jar -DpomFile=pom.xml -DlocalRepositoryPath=/Users/woodj/Documents/rewatt/mvn-repo/
3. commit and push
4. reference from your project:

```
<repositories>
    <repository>
        <id>RewattRepo</id>
        <url>https://raw.githubusercontent.com/rewattpower/mvn-repo/master</url>
    </repository>
</repositories>
...
<dependency>
    <groupId>com.googlecode.objectify</groupId>
    <artifactId>objectify</artifactId>
    <version>6.1-SNAPSHOT</version>
</dependency>
```

