# Accelerator Log

## Options
```json
{
  "createResourceClaim" : true,
  "dbType" : "Postgresql",
  "projectName" : "spring-music-for-kip",
  "workloadNamespace" : "dev"
}
```
## Log
```
┏ engine (Chain)
┃  Info Running Chain(GeneratorValidationTransform, UniquePath)
┃ ┏ ┏ engine.transformations[0].validated (Combo)
┃ ┃ ┃  Info Combo running as Let(symbols, in: Chain(Merge(merge), UniquePath(UseLast)))
┃ ┃ ┃ engine.transformations[0].validated.merge (Let)
┃ ┃ ┃ Debug Adding symbol secretName with value 'postgresql-secret'
┃ ┃ ┃ Debug Adding symbol dbName with value 'music'
┃ ┃ ┃ Debug Adding symbol dbUser with value 'postgres'
┃ ┃ ┃ Debug Adding symbol dbPassword with value 'postgres'
┃ ┃ ┃ Debug Adding symbol dbHost with value 'postgresql-music'
┃ ┃ ┃ ┏ engine.transformations[0].validated.merge.in (Chain)
┃ ┃ ┃ ┃  Info Running Chain(Merge, UniquePath)
┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.merge.in.transformations[0] (Merge)
┃ ┃ ┃ ┃ ┃  Info Running Merge(Combo, Combo, Combo, Combo)
┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.merge.in.transformations[0].sources[0] (Combo)
┃ ┃ ┃ ┃ ┃ ┃  Info Combo running as Exclude
┃ ┃ ┃ ┃ ┃ ┃ engine.transformations[0].validated.merge.in.transformations[0].sources[0].exclude (Exclude)
┃ ┃ ┃ ┃ ┃ ┃  Info Will exclude [**/templates/**]
┃ ┃ ┃ ┃ ┃ ┃ Debug .DS_Store didn't match [**/templates/**] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug .gitattributes didn't match [**/templates/**] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug .gitignore didn't match [**/templates/**] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug .tanzuignore didn't match [**/templates/**] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug .vscode/settings.json didn't match [**/templates/**] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug LICENSE didn't match [**/templates/**] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug README.md didn't match [**/templates/**] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug apply_workload.sh didn't match [**/templates/**] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/.DS_Store didn't match [**/templates/**] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/albums.json didn't match [**/templates/**] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/application.yml didn't match [**/templates/**] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/org/cloudfoundry/samples/music/Application.class didn't match [**/templates/**] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/org/cloudfoundry/samples/music/config/SpringApplicationContextInitializer.class didn't match [**/templates/**] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/org/cloudfoundry/samples/music/config/data/RedisConfig.class didn't match [**/templates/**] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/org/cloudfoundry/samples/music/domain/Album.class didn't match [**/templates/**] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/org/cloudfoundry/samples/music/domain/ApplicationInfo.class didn't match [**/templates/**] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/org/cloudfoundry/samples/music/domain/RandomIdGenerator.class didn't match [**/templates/**] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/org/cloudfoundry/samples/music/repositories/AlbumRepositoryPopulator.class didn't match [**/templates/**] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/org/cloudfoundry/samples/music/repositories/jpa/JpaAlbumRepository.class didn't match [**/templates/**] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/org/cloudfoundry/samples/music/repositories/mongodb/MongoAlbumRepository.class didn't match [**/templates/**] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/org/cloudfoundry/samples/music/repositories/redis/RedisAlbumRepository.class didn't match [**/templates/**] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/org/cloudfoundry/samples/music/web/AlbumController.class didn't match [**/templates/**] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/org/cloudfoundry/samples/music/web/ErrorController.class didn't match [**/templates/**] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/org/cloudfoundry/samples/music/web/InfoController.class didn't match [**/templates/**] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/static/.DS_Store didn't match [**/templates/**] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/static/css/app.css didn't match [**/templates/**] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/static/css/multi-columns-row.css didn't match [**/templates/**] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/static/img/glyphicons-halflings-white.png didn't match [**/templates/**] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/static/img/glyphicons-halflings.png didn't match [**/templates/**] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/static/img/music-icons.png didn't match [**/templates/**] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/static/index.html didn't match [**/templates/**] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/static/js/albums.js didn't match [**/templates/**] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/static/js/app.js didn't match [**/templates/**] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/static/js/errors.js didn't match [**/templates/**] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/static/js/info.js didn't match [**/templates/**] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/static/js/status.js didn't match [**/templates/**] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/static/templates/albumForm.html matched [**/templates/**] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/static/templates/albums.html matched [**/templates/**] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/static/templates/errors.html matched [**/templates/**] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/static/templates/footer.html matched [**/templates/**] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/static/templates/grid.html matched [**/templates/**] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/static/templates/header.html matched [**/templates/**] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/static/templates/list.html matched [**/templates/**] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/static/templates/status.html matched [**/templates/**] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug bin/test/org/cloudfoundry/samples/music/ApplicationTests.class didn't match [**/templates/**] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug build.gradle didn't match [**/templates/**] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug gradle/wrapper/gradle-wrapper.jar didn't match [**/templates/**] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug gradle/wrapper/gradle-wrapper.properties didn't match [**/templates/**] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug gradle.properties didn't match [**/templates/**] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug gradlew didn't match [**/templates/**] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug gradlew.bat didn't match [**/templates/**] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug manifest.yml didn't match [**/templates/**] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug music-icons.png didn't match [**/templates/**] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug project.toml didn't match [**/templates/**] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug settings.gradle didn't match [**/templates/**] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug src/.DS_Store didn't match [**/templates/**] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/.DS_Store didn't match [**/templates/**] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/org/cloudfoundry/samples/music/Application.java didn't match [**/templates/**] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/org/cloudfoundry/samples/music/config/SpringApplicationContextInitializer.java didn't match [**/templates/**] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/org/cloudfoundry/samples/music/config/data/RedisConfig.java didn't match [**/templates/**] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/org/cloudfoundry/samples/music/domain/Album.java didn't match [**/templates/**] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/org/cloudfoundry/samples/music/domain/ApplicationInfo.java didn't match [**/templates/**] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/org/cloudfoundry/samples/music/domain/RandomIdGenerator.java didn't match [**/templates/**] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/org/cloudfoundry/samples/music/repositories/AlbumRepositoryPopulator.java didn't match [**/templates/**] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/org/cloudfoundry/samples/music/repositories/jpa/JpaAlbumRepository.java didn't match [**/templates/**] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/org/cloudfoundry/samples/music/repositories/mongodb/MongoAlbumRepository.java didn't match [**/templates/**] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/org/cloudfoundry/samples/music/repositories/redis/RedisAlbumRepository.java didn't match [**/templates/**] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/org/cloudfoundry/samples/music/web/AlbumController.java didn't match [**/templates/**] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/org/cloudfoundry/samples/music/web/ErrorController.java didn't match [**/templates/**] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/org/cloudfoundry/samples/music/web/InfoController.java didn't match [**/templates/**] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/.DS_Store didn't match [**/templates/**] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/albums.json didn't match [**/templates/**] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/application.yml didn't match [**/templates/**] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/static/.DS_Store didn't match [**/templates/**] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/static/css/app.css didn't match [**/templates/**] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/static/css/multi-columns-row.css didn't match [**/templates/**] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/static/img/glyphicons-halflings-white.png didn't match [**/templates/**] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/static/img/glyphicons-halflings.png didn't match [**/templates/**] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/static/img/music-icons.png didn't match [**/templates/**] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/static/index.html didn't match [**/templates/**] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/static/js/albums.js didn't match [**/templates/**] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/static/js/app.js didn't match [**/templates/**] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/static/js/errors.js didn't match [**/templates/**] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/static/js/info.js didn't match [**/templates/**] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/static/js/status.js didn't match [**/templates/**] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/static/templates/albumForm.html matched [**/templates/**] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/static/templates/albums.html matched [**/templates/**] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/static/templates/errors.html matched [**/templates/**] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/static/templates/footer.html matched [**/templates/**] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/static/templates/grid.html matched [**/templates/**] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/static/templates/header.html matched [**/templates/**] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/static/templates/list.html matched [**/templates/**] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/static/templates/status.html matched [**/templates/**] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/org/cloudfoundry/samples/music/ApplicationTests.java didn't match [**/templates/**] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug templates/helm-values-postgres.yaml matched [**/templates/**] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug templates/oss-postgresql.yaml matched [**/templates/**] -> excluded
┃ ┃ ┃ ┃ ┃ ┗ Debug templates/workloads.yaml matched [**/templates/**] -> excluded
┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.merge.in.transformations[0].sources[1] (Combo)
┃ ┃ ┃ ┃ ┃ ┃  Info Combo running as Chain(Include, Chain(chain))
┃ ┃ ┃ ┃ ┃ ┃ engine.transformations[0].validated.merge.in.transformations[0].sources[1].<combo> (Chain)
┃ ┃ ┃ ┃ ┃ ┃  Info Running Chain(Include, Chain)
┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.merge.in.transformations[0].sources[1].<combo>.transformations[0] (Include)
┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Will include [**/templates/workloads.yaml]
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .DS_Store didn't match [**/templates/workloads.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gitattributes didn't match [**/templates/workloads.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gitignore didn't match [**/templates/workloads.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .tanzuignore didn't match [**/templates/workloads.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .vscode/settings.json didn't match [**/templates/workloads.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug LICENSE didn't match [**/templates/workloads.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug README.md didn't match [**/templates/workloads.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug apply_workload.sh didn't match [**/templates/workloads.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/.DS_Store didn't match [**/templates/workloads.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/albums.json didn't match [**/templates/workloads.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/application.yml didn't match [**/templates/workloads.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/org/cloudfoundry/samples/music/Application.class didn't match [**/templates/workloads.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/org/cloudfoundry/samples/music/config/SpringApplicationContextInitializer.class didn't match [**/templates/workloads.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/org/cloudfoundry/samples/music/config/data/RedisConfig.class didn't match [**/templates/workloads.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/org/cloudfoundry/samples/music/domain/Album.class didn't match [**/templates/workloads.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/org/cloudfoundry/samples/music/domain/ApplicationInfo.class didn't match [**/templates/workloads.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/org/cloudfoundry/samples/music/domain/RandomIdGenerator.class didn't match [**/templates/workloads.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/org/cloudfoundry/samples/music/repositories/AlbumRepositoryPopulator.class didn't match [**/templates/workloads.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/org/cloudfoundry/samples/music/repositories/jpa/JpaAlbumRepository.class didn't match [**/templates/workloads.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/org/cloudfoundry/samples/music/repositories/mongodb/MongoAlbumRepository.class didn't match [**/templates/workloads.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/org/cloudfoundry/samples/music/repositories/redis/RedisAlbumRepository.class didn't match [**/templates/workloads.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/org/cloudfoundry/samples/music/web/AlbumController.class didn't match [**/templates/workloads.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/org/cloudfoundry/samples/music/web/ErrorController.class didn't match [**/templates/workloads.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/org/cloudfoundry/samples/music/web/InfoController.class didn't match [**/templates/workloads.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/static/.DS_Store didn't match [**/templates/workloads.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/static/css/app.css didn't match [**/templates/workloads.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/static/css/multi-columns-row.css didn't match [**/templates/workloads.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/static/img/glyphicons-halflings-white.png didn't match [**/templates/workloads.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/static/img/glyphicons-halflings.png didn't match [**/templates/workloads.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/static/img/music-icons.png didn't match [**/templates/workloads.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/static/index.html didn't match [**/templates/workloads.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/static/js/albums.js didn't match [**/templates/workloads.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/static/js/app.js didn't match [**/templates/workloads.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/static/js/errors.js didn't match [**/templates/workloads.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/static/js/info.js didn't match [**/templates/workloads.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/static/js/status.js didn't match [**/templates/workloads.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/static/templates/albumForm.html didn't match [**/templates/workloads.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/static/templates/albums.html didn't match [**/templates/workloads.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/static/templates/errors.html didn't match [**/templates/workloads.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/static/templates/footer.html didn't match [**/templates/workloads.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/static/templates/grid.html didn't match [**/templates/workloads.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/static/templates/header.html didn't match [**/templates/workloads.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/static/templates/list.html didn't match [**/templates/workloads.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/static/templates/status.html didn't match [**/templates/workloads.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/test/org/cloudfoundry/samples/music/ApplicationTests.class didn't match [**/templates/workloads.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug build.gradle didn't match [**/templates/workloads.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug gradle/wrapper/gradle-wrapper.jar didn't match [**/templates/workloads.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug gradle/wrapper/gradle-wrapper.properties didn't match [**/templates/workloads.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug gradle.properties didn't match [**/templates/workloads.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug gradlew didn't match [**/templates/workloads.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug gradlew.bat didn't match [**/templates/workloads.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug manifest.yml didn't match [**/templates/workloads.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug music-icons.png didn't match [**/templates/workloads.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug project.toml didn't match [**/templates/workloads.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug settings.gradle didn't match [**/templates/workloads.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/.DS_Store didn't match [**/templates/workloads.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/.DS_Store didn't match [**/templates/workloads.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/org/cloudfoundry/samples/music/Application.java didn't match [**/templates/workloads.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/org/cloudfoundry/samples/music/config/SpringApplicationContextInitializer.java didn't match [**/templates/workloads.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/org/cloudfoundry/samples/music/config/data/RedisConfig.java didn't match [**/templates/workloads.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/org/cloudfoundry/samples/music/domain/Album.java didn't match [**/templates/workloads.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/org/cloudfoundry/samples/music/domain/ApplicationInfo.java didn't match [**/templates/workloads.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/org/cloudfoundry/samples/music/domain/RandomIdGenerator.java didn't match [**/templates/workloads.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/org/cloudfoundry/samples/music/repositories/AlbumRepositoryPopulator.java didn't match [**/templates/workloads.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/org/cloudfoundry/samples/music/repositories/jpa/JpaAlbumRepository.java didn't match [**/templates/workloads.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/org/cloudfoundry/samples/music/repositories/mongodb/MongoAlbumRepository.java didn't match [**/templates/workloads.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/org/cloudfoundry/samples/music/repositories/redis/RedisAlbumRepository.java didn't match [**/templates/workloads.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/org/cloudfoundry/samples/music/web/AlbumController.java didn't match [**/templates/workloads.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/org/cloudfoundry/samples/music/web/ErrorController.java didn't match [**/templates/workloads.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/org/cloudfoundry/samples/music/web/InfoController.java didn't match [**/templates/workloads.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/.DS_Store didn't match [**/templates/workloads.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/albums.json didn't match [**/templates/workloads.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/application.yml didn't match [**/templates/workloads.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/static/.DS_Store didn't match [**/templates/workloads.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/static/css/app.css didn't match [**/templates/workloads.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/static/css/multi-columns-row.css didn't match [**/templates/workloads.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/static/img/glyphicons-halflings-white.png didn't match [**/templates/workloads.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/static/img/glyphicons-halflings.png didn't match [**/templates/workloads.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/static/img/music-icons.png didn't match [**/templates/workloads.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/static/index.html didn't match [**/templates/workloads.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/static/js/albums.js didn't match [**/templates/workloads.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/static/js/app.js didn't match [**/templates/workloads.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/static/js/errors.js didn't match [**/templates/workloads.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/static/js/info.js didn't match [**/templates/workloads.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/static/js/status.js didn't match [**/templates/workloads.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/static/templates/albumForm.html didn't match [**/templates/workloads.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/static/templates/albums.html didn't match [**/templates/workloads.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/static/templates/errors.html didn't match [**/templates/workloads.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/static/templates/footer.html didn't match [**/templates/workloads.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/static/templates/grid.html didn't match [**/templates/workloads.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/static/templates/header.html didn't match [**/templates/workloads.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/static/templates/list.html didn't match [**/templates/workloads.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/static/templates/status.html didn't match [**/templates/workloads.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/org/cloudfoundry/samples/music/ApplicationTests.java didn't match [**/templates/workloads.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug templates/helm-values-postgres.yaml didn't match [**/templates/workloads.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug templates/oss-postgresql.yaml didn't match [**/templates/workloads.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┗ Debug templates/workloads.yaml matched [**/templates/workloads.yaml] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.merge.in.transformations[0].sources[1].<combo>.transformations[1] (Chain)
┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Running Chain(YTT, RewritePath)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.merge.in.transformations[0].sources[1].<combo>.transformations[1].transformations[0] (YTT)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug Wrote values file with json content:   {"secretName":"postgresql-secret","artifactVersion":"0.0.1-beta","dbName":"music","createResourceClaim":true,"dbUser":"postgres","dbType":"Postgresql","dbHost":"postgresql-music","artifactId":"spring-music-for-kip","projectName":"spring-music-for-kip","workloadNamespace":"dev","dbPassword":"postgres"}
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┗  Info Shelling out to YTT with args: [ytt, -f, /tmp/ytt-input14200650252481310238, --data-values-file, /tmp/accelerator-options10293827730608428921.json, --output-files, /tmp/ytt-output2806075201581577540]
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.merge.in.transformations[0].sources[1].<combo>.transformations[1].transformations[1] (RewritePath)
┃ ┃ ┃ ┃ ┃ ┗ ┗ ┗ Debug Path 'templates/workloads.yaml' matched 'templates/workloads.yaml' with groups {g0=templates/workloads.yaml} and was rewritten to 'config/workloads.yaml'
┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.merge.in.transformations[0].sources[2] (Combo)
┃ ┃ ┃ ┃ ┃ ┃  Info Condition (#createResourceClaim && ( #dbType == 'Postgresql') ) evaluated to true
┃ ┃ ┃ ┃ ┃ ┃  Info Combo running as Chain(Include, Chain(chain))
┃ ┃ ┃ ┃ ┃ ┃ engine.transformations[0].validated.merge.in.transformations[0].sources[2].<combo> (Chain)
┃ ┃ ┃ ┃ ┃ ┃  Info Condition (#createResourceClaim && ( #dbType == 'Postgresql') ) evaluated to true
┃ ┃ ┃ ┃ ┃ ┃  Info Running Chain(Include, Chain)
┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.merge.in.transformations[0].sources[2].<combo>.transformations[0] (Include)
┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Will include [**/templates/oss-postgresql.yaml]
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .DS_Store didn't match [**/templates/oss-postgresql.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gitattributes didn't match [**/templates/oss-postgresql.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gitignore didn't match [**/templates/oss-postgresql.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .tanzuignore didn't match [**/templates/oss-postgresql.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .vscode/settings.json didn't match [**/templates/oss-postgresql.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug LICENSE didn't match [**/templates/oss-postgresql.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug README.md didn't match [**/templates/oss-postgresql.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug apply_workload.sh didn't match [**/templates/oss-postgresql.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/.DS_Store didn't match [**/templates/oss-postgresql.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/albums.json didn't match [**/templates/oss-postgresql.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/application.yml didn't match [**/templates/oss-postgresql.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/org/cloudfoundry/samples/music/Application.class didn't match [**/templates/oss-postgresql.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/org/cloudfoundry/samples/music/config/SpringApplicationContextInitializer.class didn't match [**/templates/oss-postgresql.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/org/cloudfoundry/samples/music/config/data/RedisConfig.class didn't match [**/templates/oss-postgresql.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/org/cloudfoundry/samples/music/domain/Album.class didn't match [**/templates/oss-postgresql.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/org/cloudfoundry/samples/music/domain/ApplicationInfo.class didn't match [**/templates/oss-postgresql.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/org/cloudfoundry/samples/music/domain/RandomIdGenerator.class didn't match [**/templates/oss-postgresql.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/org/cloudfoundry/samples/music/repositories/AlbumRepositoryPopulator.class didn't match [**/templates/oss-postgresql.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/org/cloudfoundry/samples/music/repositories/jpa/JpaAlbumRepository.class didn't match [**/templates/oss-postgresql.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/org/cloudfoundry/samples/music/repositories/mongodb/MongoAlbumRepository.class didn't match [**/templates/oss-postgresql.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/org/cloudfoundry/samples/music/repositories/redis/RedisAlbumRepository.class didn't match [**/templates/oss-postgresql.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/org/cloudfoundry/samples/music/web/AlbumController.class didn't match [**/templates/oss-postgresql.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/org/cloudfoundry/samples/music/web/ErrorController.class didn't match [**/templates/oss-postgresql.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/org/cloudfoundry/samples/music/web/InfoController.class didn't match [**/templates/oss-postgresql.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/static/.DS_Store didn't match [**/templates/oss-postgresql.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/static/css/app.css didn't match [**/templates/oss-postgresql.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/static/css/multi-columns-row.css didn't match [**/templates/oss-postgresql.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/static/img/glyphicons-halflings-white.png didn't match [**/templates/oss-postgresql.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/static/img/glyphicons-halflings.png didn't match [**/templates/oss-postgresql.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/static/img/music-icons.png didn't match [**/templates/oss-postgresql.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/static/index.html didn't match [**/templates/oss-postgresql.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/static/js/albums.js didn't match [**/templates/oss-postgresql.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/static/js/app.js didn't match [**/templates/oss-postgresql.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/static/js/errors.js didn't match [**/templates/oss-postgresql.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/static/js/info.js didn't match [**/templates/oss-postgresql.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/static/js/status.js didn't match [**/templates/oss-postgresql.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/static/templates/albumForm.html didn't match [**/templates/oss-postgresql.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/static/templates/albums.html didn't match [**/templates/oss-postgresql.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/static/templates/errors.html didn't match [**/templates/oss-postgresql.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/static/templates/footer.html didn't match [**/templates/oss-postgresql.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/static/templates/grid.html didn't match [**/templates/oss-postgresql.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/static/templates/header.html didn't match [**/templates/oss-postgresql.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/static/templates/list.html didn't match [**/templates/oss-postgresql.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/static/templates/status.html didn't match [**/templates/oss-postgresql.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/test/org/cloudfoundry/samples/music/ApplicationTests.class didn't match [**/templates/oss-postgresql.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug build.gradle didn't match [**/templates/oss-postgresql.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug gradle/wrapper/gradle-wrapper.jar didn't match [**/templates/oss-postgresql.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug gradle/wrapper/gradle-wrapper.properties didn't match [**/templates/oss-postgresql.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug gradle.properties didn't match [**/templates/oss-postgresql.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug gradlew didn't match [**/templates/oss-postgresql.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug gradlew.bat didn't match [**/templates/oss-postgresql.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug manifest.yml didn't match [**/templates/oss-postgresql.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug music-icons.png didn't match [**/templates/oss-postgresql.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug project.toml didn't match [**/templates/oss-postgresql.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug settings.gradle didn't match [**/templates/oss-postgresql.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/.DS_Store didn't match [**/templates/oss-postgresql.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/.DS_Store didn't match [**/templates/oss-postgresql.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/org/cloudfoundry/samples/music/Application.java didn't match [**/templates/oss-postgresql.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/org/cloudfoundry/samples/music/config/SpringApplicationContextInitializer.java didn't match [**/templates/oss-postgresql.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/org/cloudfoundry/samples/music/config/data/RedisConfig.java didn't match [**/templates/oss-postgresql.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/org/cloudfoundry/samples/music/domain/Album.java didn't match [**/templates/oss-postgresql.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/org/cloudfoundry/samples/music/domain/ApplicationInfo.java didn't match [**/templates/oss-postgresql.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/org/cloudfoundry/samples/music/domain/RandomIdGenerator.java didn't match [**/templates/oss-postgresql.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/org/cloudfoundry/samples/music/repositories/AlbumRepositoryPopulator.java didn't match [**/templates/oss-postgresql.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/org/cloudfoundry/samples/music/repositories/jpa/JpaAlbumRepository.java didn't match [**/templates/oss-postgresql.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/org/cloudfoundry/samples/music/repositories/mongodb/MongoAlbumRepository.java didn't match [**/templates/oss-postgresql.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/org/cloudfoundry/samples/music/repositories/redis/RedisAlbumRepository.java didn't match [**/templates/oss-postgresql.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/org/cloudfoundry/samples/music/web/AlbumController.java didn't match [**/templates/oss-postgresql.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/org/cloudfoundry/samples/music/web/ErrorController.java didn't match [**/templates/oss-postgresql.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/org/cloudfoundry/samples/music/web/InfoController.java didn't match [**/templates/oss-postgresql.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/.DS_Store didn't match [**/templates/oss-postgresql.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/albums.json didn't match [**/templates/oss-postgresql.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/application.yml didn't match [**/templates/oss-postgresql.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/static/.DS_Store didn't match [**/templates/oss-postgresql.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/static/css/app.css didn't match [**/templates/oss-postgresql.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/static/css/multi-columns-row.css didn't match [**/templates/oss-postgresql.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/static/img/glyphicons-halflings-white.png didn't match [**/templates/oss-postgresql.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/static/img/glyphicons-halflings.png didn't match [**/templates/oss-postgresql.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/static/img/music-icons.png didn't match [**/templates/oss-postgresql.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/static/index.html didn't match [**/templates/oss-postgresql.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/static/js/albums.js didn't match [**/templates/oss-postgresql.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/static/js/app.js didn't match [**/templates/oss-postgresql.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/static/js/errors.js didn't match [**/templates/oss-postgresql.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/static/js/info.js didn't match [**/templates/oss-postgresql.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/static/js/status.js didn't match [**/templates/oss-postgresql.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/static/templates/albumForm.html didn't match [**/templates/oss-postgresql.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/static/templates/albums.html didn't match [**/templates/oss-postgresql.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/static/templates/errors.html didn't match [**/templates/oss-postgresql.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/static/templates/footer.html didn't match [**/templates/oss-postgresql.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/static/templates/grid.html didn't match [**/templates/oss-postgresql.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/static/templates/header.html didn't match [**/templates/oss-postgresql.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/static/templates/list.html didn't match [**/templates/oss-postgresql.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/static/templates/status.html didn't match [**/templates/oss-postgresql.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/org/cloudfoundry/samples/music/ApplicationTests.java didn't match [**/templates/oss-postgresql.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug templates/helm-values-postgres.yaml didn't match [**/templates/oss-postgresql.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug templates/oss-postgresql.yaml matched [**/templates/oss-postgresql.yaml] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┗ Debug templates/workloads.yaml didn't match [**/templates/oss-postgresql.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.merge.in.transformations[0].sources[2].<combo>.transformations[1] (Chain)
┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Running Chain(YTT, RewritePath)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.merge.in.transformations[0].sources[2].<combo>.transformations[1].transformations[0] (YTT)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug Wrote values file with json content:   {"secretName":"postgresql-secret","artifactVersion":"0.0.1-beta","dbName":"music","createResourceClaim":true,"dbUser":"postgres","dbType":"Postgresql","dbHost":"postgresql-music","artifactId":"spring-music-for-kip","projectName":"spring-music-for-kip","workloadNamespace":"dev","dbPassword":"postgres"}
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┗  Info Shelling out to YTT with args: [ytt, -f, /tmp/ytt-input3842239147419829308, --data-values-file, /tmp/accelerator-options1233240844901788179.json, --output-files, /tmp/ytt-output15960789893866280167]
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.merge.in.transformations[0].sources[2].<combo>.transformations[1].transformations[1] (RewritePath)
┃ ┃ ┃ ┃ ┃ ┗ ┗ ┗ Debug Path 'templates/oss-postgresql.yaml' matched 'templates/oss-postgresql.yaml' with groups {g0=templates/oss-postgresql.yaml} and was rewritten to 'config/postgresql/oss-postgresql.yaml'
┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.merge.in.transformations[0].sources[3] (Combo)
┃ ┃ ┃ ┃ ┃ ┃  Info Combo running as Chain(Include, Chain(chain))
┃ ┃ ┃ ┃ ┃ ┃ engine.transformations[0].validated.merge.in.transformations[0].sources[3].<combo> (Chain)
┃ ┃ ┃ ┃ ┃ ┃  Info Running Chain(Include, Chain)
┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.merge.in.transformations[0].sources[3].<combo>.transformations[0] (Include)
┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Will include [**/templates/helm-values-postgres.yaml]
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .DS_Store didn't match [**/templates/helm-values-postgres.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gitattributes didn't match [**/templates/helm-values-postgres.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gitignore didn't match [**/templates/helm-values-postgres.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .tanzuignore didn't match [**/templates/helm-values-postgres.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .vscode/settings.json didn't match [**/templates/helm-values-postgres.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug LICENSE didn't match [**/templates/helm-values-postgres.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug README.md didn't match [**/templates/helm-values-postgres.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug apply_workload.sh didn't match [**/templates/helm-values-postgres.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/.DS_Store didn't match [**/templates/helm-values-postgres.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/albums.json didn't match [**/templates/helm-values-postgres.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/application.yml didn't match [**/templates/helm-values-postgres.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/org/cloudfoundry/samples/music/Application.class didn't match [**/templates/helm-values-postgres.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/org/cloudfoundry/samples/music/config/SpringApplicationContextInitializer.class didn't match [**/templates/helm-values-postgres.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/org/cloudfoundry/samples/music/config/data/RedisConfig.class didn't match [**/templates/helm-values-postgres.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/org/cloudfoundry/samples/music/domain/Album.class didn't match [**/templates/helm-values-postgres.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/org/cloudfoundry/samples/music/domain/ApplicationInfo.class didn't match [**/templates/helm-values-postgres.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/org/cloudfoundry/samples/music/domain/RandomIdGenerator.class didn't match [**/templates/helm-values-postgres.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/org/cloudfoundry/samples/music/repositories/AlbumRepositoryPopulator.class didn't match [**/templates/helm-values-postgres.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/org/cloudfoundry/samples/music/repositories/jpa/JpaAlbumRepository.class didn't match [**/templates/helm-values-postgres.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/org/cloudfoundry/samples/music/repositories/mongodb/MongoAlbumRepository.class didn't match [**/templates/helm-values-postgres.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/org/cloudfoundry/samples/music/repositories/redis/RedisAlbumRepository.class didn't match [**/templates/helm-values-postgres.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/org/cloudfoundry/samples/music/web/AlbumController.class didn't match [**/templates/helm-values-postgres.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/org/cloudfoundry/samples/music/web/ErrorController.class didn't match [**/templates/helm-values-postgres.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/org/cloudfoundry/samples/music/web/InfoController.class didn't match [**/templates/helm-values-postgres.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/static/.DS_Store didn't match [**/templates/helm-values-postgres.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/static/css/app.css didn't match [**/templates/helm-values-postgres.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/static/css/multi-columns-row.css didn't match [**/templates/helm-values-postgres.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/static/img/glyphicons-halflings-white.png didn't match [**/templates/helm-values-postgres.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/static/img/glyphicons-halflings.png didn't match [**/templates/helm-values-postgres.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/static/img/music-icons.png didn't match [**/templates/helm-values-postgres.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/static/index.html didn't match [**/templates/helm-values-postgres.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/static/js/albums.js didn't match [**/templates/helm-values-postgres.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/static/js/app.js didn't match [**/templates/helm-values-postgres.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/static/js/errors.js didn't match [**/templates/helm-values-postgres.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/static/js/info.js didn't match [**/templates/helm-values-postgres.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/static/js/status.js didn't match [**/templates/helm-values-postgres.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/static/templates/albumForm.html didn't match [**/templates/helm-values-postgres.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/static/templates/albums.html didn't match [**/templates/helm-values-postgres.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/static/templates/errors.html didn't match [**/templates/helm-values-postgres.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/static/templates/footer.html didn't match [**/templates/helm-values-postgres.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/static/templates/grid.html didn't match [**/templates/helm-values-postgres.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/static/templates/header.html didn't match [**/templates/helm-values-postgres.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/static/templates/list.html didn't match [**/templates/helm-values-postgres.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/main/static/templates/status.html didn't match [**/templates/helm-values-postgres.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug bin/test/org/cloudfoundry/samples/music/ApplicationTests.class didn't match [**/templates/helm-values-postgres.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug build.gradle didn't match [**/templates/helm-values-postgres.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug gradle/wrapper/gradle-wrapper.jar didn't match [**/templates/helm-values-postgres.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug gradle/wrapper/gradle-wrapper.properties didn't match [**/templates/helm-values-postgres.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug gradle.properties didn't match [**/templates/helm-values-postgres.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug gradlew didn't match [**/templates/helm-values-postgres.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug gradlew.bat didn't match [**/templates/helm-values-postgres.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug manifest.yml didn't match [**/templates/helm-values-postgres.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug music-icons.png didn't match [**/templates/helm-values-postgres.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug project.toml didn't match [**/templates/helm-values-postgres.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug settings.gradle didn't match [**/templates/helm-values-postgres.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/.DS_Store didn't match [**/templates/helm-values-postgres.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/.DS_Store didn't match [**/templates/helm-values-postgres.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/org/cloudfoundry/samples/music/Application.java didn't match [**/templates/helm-values-postgres.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/org/cloudfoundry/samples/music/config/SpringApplicationContextInitializer.java didn't match [**/templates/helm-values-postgres.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/org/cloudfoundry/samples/music/config/data/RedisConfig.java didn't match [**/templates/helm-values-postgres.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/org/cloudfoundry/samples/music/domain/Album.java didn't match [**/templates/helm-values-postgres.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/org/cloudfoundry/samples/music/domain/ApplicationInfo.java didn't match [**/templates/helm-values-postgres.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/org/cloudfoundry/samples/music/domain/RandomIdGenerator.java didn't match [**/templates/helm-values-postgres.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/org/cloudfoundry/samples/music/repositories/AlbumRepositoryPopulator.java didn't match [**/templates/helm-values-postgres.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/org/cloudfoundry/samples/music/repositories/jpa/JpaAlbumRepository.java didn't match [**/templates/helm-values-postgres.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/org/cloudfoundry/samples/music/repositories/mongodb/MongoAlbumRepository.java didn't match [**/templates/helm-values-postgres.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/org/cloudfoundry/samples/music/repositories/redis/RedisAlbumRepository.java didn't match [**/templates/helm-values-postgres.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/org/cloudfoundry/samples/music/web/AlbumController.java didn't match [**/templates/helm-values-postgres.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/org/cloudfoundry/samples/music/web/ErrorController.java didn't match [**/templates/helm-values-postgres.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/org/cloudfoundry/samples/music/web/InfoController.java didn't match [**/templates/helm-values-postgres.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/.DS_Store didn't match [**/templates/helm-values-postgres.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/albums.json didn't match [**/templates/helm-values-postgres.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/application.yml didn't match [**/templates/helm-values-postgres.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/static/.DS_Store didn't match [**/templates/helm-values-postgres.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/static/css/app.css didn't match [**/templates/helm-values-postgres.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/static/css/multi-columns-row.css didn't match [**/templates/helm-values-postgres.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/static/img/glyphicons-halflings-white.png didn't match [**/templates/helm-values-postgres.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/static/img/glyphicons-halflings.png didn't match [**/templates/helm-values-postgres.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/static/img/music-icons.png didn't match [**/templates/helm-values-postgres.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/static/index.html didn't match [**/templates/helm-values-postgres.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/static/js/albums.js didn't match [**/templates/helm-values-postgres.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/static/js/app.js didn't match [**/templates/helm-values-postgres.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/static/js/errors.js didn't match [**/templates/helm-values-postgres.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/static/js/info.js didn't match [**/templates/helm-values-postgres.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/static/js/status.js didn't match [**/templates/helm-values-postgres.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/static/templates/albumForm.html didn't match [**/templates/helm-values-postgres.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/static/templates/albums.html didn't match [**/templates/helm-values-postgres.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/static/templates/errors.html didn't match [**/templates/helm-values-postgres.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/static/templates/footer.html didn't match [**/templates/helm-values-postgres.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/static/templates/grid.html didn't match [**/templates/helm-values-postgres.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/static/templates/header.html didn't match [**/templates/helm-values-postgres.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/static/templates/list.html didn't match [**/templates/helm-values-postgres.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/static/templates/status.html didn't match [**/templates/helm-values-postgres.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/org/cloudfoundry/samples/music/ApplicationTests.java didn't match [**/templates/helm-values-postgres.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug templates/helm-values-postgres.yaml matched [**/templates/helm-values-postgres.yaml] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug templates/oss-postgresql.yaml didn't match [**/templates/helm-values-postgres.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┗ Debug templates/workloads.yaml didn't match [**/templates/helm-values-postgres.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.merge.in.transformations[0].sources[3].<combo>.transformations[1] (Chain)
┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Running Chain(YTT, RewritePath)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.merge.in.transformations[0].sources[3].<combo>.transformations[1].transformations[0] (YTT)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug Wrote values file with json content:   {"secretName":"postgresql-secret","artifactVersion":"0.0.1-beta","dbName":"music","createResourceClaim":true,"dbUser":"postgres","dbType":"Postgresql","dbHost":"postgresql-music","artifactId":"spring-music-for-kip","projectName":"spring-music-for-kip","workloadNamespace":"dev","dbPassword":"postgres"}
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┗  Info Shelling out to YTT with args: [ytt, -f, /tmp/ytt-input1329676318297027684, --data-values-file, /tmp/accelerator-options2898886486285964512.json, --output-files, /tmp/ytt-output2476407884649742795]
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.merge.in.transformations[0].sources[3].<combo>.transformations[1].transformations[1] (RewritePath)
┃ ┃ ┃ ┃ ┗ ┗ ┗ ┗ Debug Path 'templates/helm-values-postgres.yaml' matched 'templates/helm-values-postgres.yaml' with groups {g0=templates/helm-values-postgres.yaml} and was rewritten to 'config/helm/helm-values-postgres.yaml'
┃ ┗ ┗ ┗ ╺ engine.transformations[0].validated.merge.in.transformations[1] (UniquePath)
┗ ╺ engine.transformations[1] (UniquePath)
```
