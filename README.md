# mvn-repo
Custom maven artifacts

# Creating a modified 3rd party jar

1. Fork a repo
2. Clone it
3. Make changes
4. Commit and push changes
5. Make a PR, ideally

# Publishing your jar

1. mvn package
2. mvn install:install-file -Dfile=target/objectify-6.1-SNAPSHOT.jar -DpomFile=pom.xml -DlocalRepositoryPath=/Users/woodj/Documents/rewatt/mvn-repo/
3. commit and push
4. reference from your project:

