# gradle-copy-example

## To reproduce locally

1. Clone this repo
2. Open `build.gradle` and modify the `deploy` task to suit your particular system by changing `PATH_TO_YOUR_USERHOME` to a valid path that your user has write access to. I'm on a Mac, so in my case the `PATH_TO_YOUR_USERHOME` is `/Users/myuser`, etc.
3. Navigate back to the project root
4. Run `./gradlew clean build shadowJar deploy`

Go to the `/PATH_TO_YOUR_USERHOME/tmp/deploy`. You will only see the JAR has been copied (`gradlecopyexample.jar`), and not the `config` directory.
