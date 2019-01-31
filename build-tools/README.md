# Build Tools demo

This folder contains a simple Spring Boot application.

> Note: A working JDK8+ is required to perform build with Gradle or Maven

## Gradle

This demo will use the Gradle wrapper.

### Display available Tasks

Linux

```sh
./gradlew tasks
```

Windows

```sh
gradlew.bat tasks
```

### Test with Gradle

Linux

```sh
./gradlew test
```

Windows

```sh
gradlew.bat test
```

The test reports are available after the test run in the `build/reports` directory. Check the `index.html` for a detailed report.

### Build with Gradle

Linux

```sh
./gradlew build
```

Windows

```sh
gradlew.bat build
```

The artifact is available after the build in the `build/libs` folder.

### Start application with Gradle

After the build the application can be started using Gradle or Java `java -jar spring-boot-demo-gradle-0.1.0.jar`

If the application startup fails due to a port colission, change the port in the [`application.properties`](src/main/resources/application.properties) file.

By default the application is reachable in your browser via [http://localhost:8080](http://localhost:8080)

> Note: If you changed the port, this link will not work, you have to change the port here as well.

Linux

```sh
./gradlew bootRun
```

Windows

```sh
gradlew.bat bootRun
```

## Maven

This demo will use the Maven wrapper.

### Display available Goals

Linux

```sh
./gradlew tasks
```

Windows

```sh
gradlew.bat tasks
```

### Test with Maven

Linux

```sh
./mvnw test
```

Windows

```sh
mvnw.cmd test
```

The test reports are available after the test run in the `target/surefire-reports` directory. Check the `com.example.hello.HelloControllerTest.txt` for a test report.

### Build with Maven

Linux

```sh
./mvnw package
```

Windows

```sh
mvnw.cmd package
```

The artifact is available after the build in the `target` folder.

### Start application

After the build the application can be started using Maven or Java `java -jar spring-boot-demo-maven-0.1.0.jar`

If the application startup fails due to a port colission, change the port in the [`application.properties`](src/main/resources/application.properties) file.

By default the application is reachable in your browser via [http://localhost:8080](http://localhost:8080)

> Note: If you changed the port, this link will not work, you have to change the port here as well.

Linux

```sh
./mvnw run
```

Windows

```sh
mvnw.cmd run
```