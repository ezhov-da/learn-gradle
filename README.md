# learn-gradle
Learn Gradle


[https://github.com/gradle/gradle](https://github.com/gradle/gradle)
[https://habr.com/ru/post/167227/](https://habr.com/ru/post/167227/)
[https://habr.com/ru/post/458046/](https://habr.com/ru/post/458046/)

## Вызов задач

```
./gradlew tasks                         # доступные задачи
./gradlew subprojectName:tasks --all    # все задачи, включая второстепенные
./gradlew app:assembleDevelopDebug      # вызваны все задачи, от которых она зависит
./gradlew app:assembleDD                # лень писать название целиком, можно выкинуть маленькие буковки
```

## Логгинг

```
# -q, -w, -i, -d  или --quiet, --warn, --info, --debug, stacktrace опция -s
./gradlew app:build -d > myLog.txt
```