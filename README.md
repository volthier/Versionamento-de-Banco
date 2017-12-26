# Versionamento De Banco de Dados.

Esse repositório aborda o uso da biblioteca **[Liquibase](http://www.liquibase.org/index.html)** de codigo aberto. Especialemnte utilizada em ambientes de desenvolvimento ágil para mapeamento, monitoramento e aplicação de mudanças em esquemas de base de dados.

## Liquibase 

> **Suporta:** *MySQL,	PostgreSQL, Oracle_11g, Sql_Server, Sybase_Enterprise, Sybase_Anywhere, DB2, Apache_Derby, HSQL, H2,	Informix, Firebird e SQLite.*


https://imasters.com.br/artigo/13991/banco-de-dados/refactoring-de-banco-de-dados-com-liquibase-parte-01-conceitos/?trace=1519021197&source=single

https://www.sitepoint.com/versioning-your-database-with-liquibase/

https://dicasdolampada.wordpress.com/2012/03/19/evoluindo-o-banco-de-dados-com-o-liquibase/




Liquibase scripts can be written in multiple formats like JSON, XML, YAML etc that are agnostic to the actual database. This makes it quite easy to migrate the application from one relational database to another with Liquibase doing the heavy-lifting for  translating the Liquibase scripts to the database specific SQLs.

Liquibase consists of change sets which are basically a small set of changes applied to the database. Liquibase tracks the execution of the change sets and records them in a change log table. Change sets can be created representing multiple releases and organized in a sequential order in the change log file. This allows for versioning the database updates and maintaining all the scripts in a central location. Whenever a change needs to be applied to database, we can create a new change set and add it to the change log. This allows for having an immutable log of all the database schema changes and minimizes any risk of inadvertently applying a wrong patch during application install or database migration.
