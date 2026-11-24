# JAVA-Stock-Portfolio
This JAVA project aims to build a stock portfolio for people to use to monitor any stocks or ETFs a user may have.

A command-line stock portfolio and trading simulator written in Java, built to practice
object-oriented design: abstract asset types (stocks, ETFs, bonds), polymorphic order
types, custom exceptions, and generic repositories.

## Run it
Requires Java 17+ and Maven.

```
mvn compile exec:java -Dexec.mainClass=com.brian.portfolio.Main   # or run Main from your IDE
mvn test
```

## Database
In Phase 7 this app connects to a MySQL 8 database designed in the companion project,
[SQL-Brokerage-database](https://github.com/brianbermudez0489-bot/SQL-Brokerage-database).
Securities are loaded from it, trades are saved to it, and reports run its views and
window-function queries.

## Progress
See [ROADMAP.md](ROADMAP.md).
