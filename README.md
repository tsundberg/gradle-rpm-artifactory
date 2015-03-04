# gradle-rpm-artifactory
An example of a Gradle project that should deliver an rpm to a yum repo hosted on an Artifactory-Pro

Build the binaries and upload the rpm:

```
gradle deployRpm
```

in the project root directory

Install the application on a RedHat box that is aware of the yum repository used in the deployRpm task.

```
yum install gradle-rpm-artifactory
```

The missing part in this example is the implementation of the uploadRpm task.
It needs to be added and we hope that a pull request from the JFrog support
team will help us with this.
