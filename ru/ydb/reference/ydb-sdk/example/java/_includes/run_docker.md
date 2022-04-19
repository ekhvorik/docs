---
sourcePath: ru/ydb/ydb-docs-core/ru/core/reference/ydb-sdk/example/java/_includes/run_docker.md
---
Для соединения с развернутой локальной базой данных YDB по сценарию [Docker](../../../../../getting_started/self_hosted/ydb_docker.md) в конфигурации по умолчанию  выполните следующую команду:

``` bash
(cd ydb-java-sdk/examples/basic_example/target && \
YDB_ANONYMOUS_CREDENTIALS=1 java -jar ydb-basic-example.jar grpc://localhost:2136?database=/local )
```