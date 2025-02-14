---
pill: password
subtitle: flyway.password
redirect_from: Configuration/password/
---

# Password

## Description
The password to use to connect to the database

This can be omitted if the password is baked into the [url](Configuration/parameters/url) (See [Sql Server](Supported Databases/SQL Server#windows-authentication) for an example), or if password is provided through another means (such as [aws secrets](Configuration/Secrets Management)).

## Usage

### Commandline
```powershell
./flyway -password=mysecretpassword info
```

### Configuration File
```properties
flyway.password=mysecretpassword
```

### Environment Variable
```properties
FLYWAY_PASSWORD=mysecretpassword
```

### API
```java
Flyway.configure()
    .password("mysecretpassword")
    .load()
```

### Gradle
```groovy
flyway {
    password = 'mysecretpassword'
}
```

### Maven
```xml
<configuration>
    <password>mysecretpassword</password>
</configuration>
```
