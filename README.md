# ai-docs

## Сборка

```bash
mvn clean package -DskipTests
```

## Запуск в Git Bash

```bash
export OPENAI_API_KEY="<ВАШ_API_KEY>"
```

```bash
java -Djavax.net.ssl.trustStore=/c/PROGRA~1/Java/jdk-21/lib/security/cacerts \
     -Djavax.net.ssl.trustStorePassword=changeit \
     -Djavax.net.ssl.trustStoreType=JKS \
     -jar target/ai-docs-1.0-SNAPSHOT.jar
```

## Использование

После запуска введите:

```text
help
```

чтобы увидеть список доступных команд.

Пример команды:

```text
>q "What is Spring Boot?"
```
### 1. Узнайте PID процесса

В Git Bash выполните:

```bash
netstat -ano | grep ':8080'
```

Пример вывода:

```text
TCP    0.0.0.0:8080    0.0.0.0:0    LISTENING    12345
```

Последнее число в строке — это PID процесса.

В этом примере PID:

```text
12345
```
### 2. Остановите процесс

В Git Bash выполните:

```bash
taskkill //F //PID 12345
```

Вместо `12345` подставьте свой PID.

Важно: в Git Bash нужно использовать двойные слеши `//`, а не одиночные `/`.