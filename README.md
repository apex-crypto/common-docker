PEAK6 for ARM64

run

```
mvn clean install \
  -DskipTests -Pdocker \
  -Ddocker.registry=arm/
```

You may need to modify your .m2 config
when maven is installed via sdkman
`/Users/efabens/.sdkman/candidates/maven/current/conf/settings.xml`

comment out the following mirror
```
    <mirror>
      <id>maven-default-http-blocker</id>
      <mirrorOf>external:http:*</mirrorOf>
      <name>Pseudo repository to mirror external repositories initially using HTTP.</name>
      <url>http://0.0.0.0/</url>
      <blocked>true</blocked>
    </mirror>
```

# Common Docker Utilities

See [base image](./base/README.md), [utility belt](./utility-belt/README.md)
