

[Udemy Spring Boot Course](https://www.udemy.com/spring-boot-intro/learn/v4/t/lecture/3956862?start=0)

[course code](https://github.com/danvega/spring-boot-intro)

[Spring Boot Docs](http://docs.spring.io/spring-boot/docs/current/ref)

[Spring Boot API](http://docs.spring.io/spring-boot/docs/current/api)

[Spring IO Platform](http://spring.io/projects)

[Spring Tools](https://spring.io/tools)

[Getting Started Guides](http://spring.io/guides)

[Java SE Development Kit 8 Downloads](https://www.oracle.com/technetwork/java/javase/downloads/jdk8-downloads-2133151.html)

## Verify Running Latest Java

```
java -version
```

* System Preferences
* Java
* Update

Shows I am running the latest.

Ensure `Check for Updates Automatically` is Checked

## Install STS

[Spring Tools](https://spring.io/tools)

* Download STS4, macOS 64-bit
* Install

## Install Maven

[Maven](http://maven.apache.org/)

* Downloaded 3.6.0
* Copied to `/Users/⁨jv/⁨Desktop/⁨OtherTools⁩/apache-maven`

Set `M2_HOME`

```
M2_HOME=/Users/jv/Desktop/OtherTools/apache-maven
```

Check the version

```
mvn -v
```


## Install Ant

[Apache Ant](https://ant.apache.org)

* Download `apache-ant-1.10.5-bin.tar.gz`
* Download KEYS
* Download PGP `apache-ant-1.10.5-bin.tar.gz.asc`

```
gpg --import KEYS
gpg --verify apache-ant-1.10.5-bin.tar.gz.asc
```

```
gunzip apache-ant-1.10.5-bin.tar.gz
```

copy `apache-ant-1.10.5` to `/Users/jv/Desktop/OtherTools/apache-ant`

Set `ANT_HOME=/Users/jv/Desktop/OtherTools/apache-ant`

```
ant -v
```

## Install Gradle

[Gradle](https://gradle.org/)

[Gradle Install](https://gradle.org/install/)

[Gradle Chearsheet](https://devhints.io/homebrew)

```
brew list
brew list --versions gradle
```

shows Gradle is already installed.

```
gradle -v
```

```
Gradle 2.11
```

## Install Spring Boot CLI

```
brew tap pivotal/tap
brew install springboot
```

```
brew list
```

Homebrew installs `spring` to `/usr/local/bin`

### Spring CLI

```
spring version
spring help run
```

## Simple Project

`repo-spring-boot/simple-1`

`app.groovy`

```
@RestController
public class HelloWorld {
	
	@RequestMapping("/")
	public String home() {
	"Hello World"
	}
}
```

```
spring run app.groovy
```

```
http://localhost:8080/
```






