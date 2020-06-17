# JFlex - runnable with IntelliJ
This project offers an executable version of "ÜB-Praxis-JFlex Scanner for AS-Leer". 
Further tasks, solutions and packages have to be inserted with the course of the lecture itself.
To generate a lexer file, you must specify it in the POM.
```xml
    <configuration>
        <lexDefinitions>
            <lexDefinition>src/main/java/de/dhbw/compiler/jflexasscanner/JFlexASScanner.lex</lexDefinition>
        </lexDefinitions>
    </configuration>
```
The scanner is regenerated with *mvn install* and can be found in *target/generated-sources/jflex/de/dhbw/compiler/jflexasscanner*.
It might occur that you have to mark *target/generated-sources/jflex* as *generated-resources-root* so it's recognized by any test or class. 
