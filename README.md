## Microbenchmarking using JMH

Set GraalVM
```shell script
$ sdk use java 19.3.0.r11-grl
$ java -version
openjdk version "11.0.5" 2019-10-15
OpenJDK Runtime Environment (build 11.0.5+10-jvmci-19.3-b05-LTS)
OpenJDK 64-Bit GraalVM CE 19.3.0 (build 11.0.5+10-jvmci-19.3-b05-LTS, mixed mode, sharing)
```

Set OpenJDK 14-ea
```shell script
$ sdk use java 14.ea.24-open
$ java -version
openjdk version "14-ea" 2020-03-17
OpenJDK Runtime Environment (build 14-ea+24-1107)
OpenJDK 64-Bit Server VM (build 14-ea+24-1107, mixed mode, sharing)
```

Generate the benchmark JAR
```shell script
mvn clean install
```

Run the benchmark
```shell script
java -jar targets/benchmarks.jar
```