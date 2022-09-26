## Build with Gradle

#### To let gradle know about all modules in project run in Terminal:
> ./gradlew projects
#### Just build project:
> ./gradlew clean build

### to build war artifact via Gradle
> ./gradlew war

### to run test via Gradle
> ./gradlew testClasses

### to clean all build artifacts from project structure
> ./gradlew clean


## Build via Maven

### Build project via Maven
In parent project, uses the standard mvn compile to compile all the modules, Maven will decide the build order.
> mvn compile

### Compile the web module only
> mvn -pl web compile

### Compile specified modules
> mvn -pl +admin,+web compile

### Run test via Maven
> mvn -pl +admin,+web clean test

### Create jar & war artifacts 
> mvn package

The type of artifact this project produces is pointed in tags 'packaging'

### To delete the target directory/es
> mvn clean
