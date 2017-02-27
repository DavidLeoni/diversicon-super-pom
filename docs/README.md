<p class="josman-to-strip">
WARNING: WORK IN PROGRESS - THIS IS ONLY A TEMPLATE FOR THE DOCUMENTATION. <br/>
RELEASE DOCS ARE ON THE <a href="http://diversicon-kb.eu/manual/diversicon-super-pom/" target="_blank">PROJECT WEBSITE</a>
</p>


### Getting started

If you use Maven as build system, put this in the `dependencies` section of your `pom.xml`:

```xml
    <dependency>
        <groupId>eu.kidf</groupId>
        <artifactId>diversicon-super-pom</artifactId>
        <version>${project.version}</version>
    </dependency>
```

If you want to use Wordnet 3.1, you have to add this additional dependency:

```xml
	<dependency>
		<groupId>eu.kidf</groupId>
		<artifactId>div-wn31-h2db</artifactId>
		<version>${project.version}</version>		
	</dependency>

```

### Example Usage

To create a database with Wordnet 3.1 and then import the example resource Smartphones, you can
look at the example [`TestApp1`](../../src/test/java/eu/kidf/diversicon/core/test/TestApp1.java) 

For more usage examples, you can have a look at DiverCLI project, in particular the various [Commands](https://github.com/diversicon-kb/divercli/tree/master/src/main/java/eu/kidf/diversicon/cli/commands)

### Logging

Diversicon uses <a href="http://www.slf4j.org" target="_blank">SLF4J </a> logging system. Library has only `slf4j-api` as dependency. For using logging during development / testing, see [the wiki](../../../wiki/#logging).