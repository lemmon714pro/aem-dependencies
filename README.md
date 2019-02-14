aem-dependencies
================

Utility project provides maven dependencies for Adobe AEM/CQ5.

Each pom file should be installed using Maven:
'''mvn -f pom-6.4.xml clean install
mvn -f pom-5.6.1.xml clean install'''

Then in your project pom you can use installed artifacts:
'''    <properties>
        <cq.version>6.4</cq.version>
    </properties>
    <dependency>
        <groupId>com.yurishchev.aem</groupId>
        <artifactId>aem-dependencies</artifactId>
        <version>${cq.version}</version>
        <type>pom</type>
        <scope>import</scope>
    </dependency>
'''
