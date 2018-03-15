# JAVA_livrable_001

1- Créer l'arborescence:

ex:
mkdir -p JAVA_livrable_001/src/main/java/hello666

2- Créer le pom.xml

ex:

<?xml version="1.0" encoding="UTF-8"?>
<project>
 <modelVersion>4.0.0</modelVersion>
 <groupId>fr.campus-numerique-in-the-alps</groupId>
 <artifactId>hello666</artifactId>
 <version>1</version>
 <properties>
   <maven.compiler.source>1.8</maven.compiler.source>
   <maven.compiler.target>1.8</maven.compiler.target>
   <project.build.sourceEncoding>UTF-8</project.build.sourceEncoding>
 </properties>
</project>


3- Créer les fichiers .java dans le dossier java.

ex: HelloAgain.java

package hello666;

public class HelloAgain {
   public static void main(String[] args) {
       System.out.println("Coucou");
   }
}
NB: System.out.println("Test !!!"); est “ce qui s’exécute”.

4- mvn:

mvn compile 
mvn install
java -cp target/hello666-1.jar hello666.HelloAgain

On exécute dans le hello666-1.jar la classe HelloAgain qui fait partie du package hello666.
NB: le “1” est la version que l’on appelle.
