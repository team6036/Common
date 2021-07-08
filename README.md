# Common

Common library for 6036 code

## Contents

* Gyroscope Encapsulation
* Odometry for Swerve (Currently Innacurate)
* Swerve Controller
* Swerve Constants
* Vector Libary
* Pose Library to Complement Vector Library (Not to be Confused With Pose2d)
* General Math Utilities for Trignonmetry, Kinematics, Simulation, Profiling, Etc.

## How to use in another project

The Common library is imported into a project by using
[Git submodules](https://git-scm.com/book/en/v2/Git-Tools-Submodules). In
order to add this project as a submodule run `git submodule add
https://github.com/team6036/Common.git Common` in your project's root
directory. This will clone this repository into the directory `Common`.

### Using the Common library

A dependency on the robot library can be created by adding the following to
your `build.gradle` file:

```gradle
plugins {
    ...
    id 'edu.wpi.first.GradleRIO' version '2020.1.2'
    ...
}
...
dependencies {
    ...
    compile project(':Common')
    ...
}
```

> NOTE: The common library does not need to be an explicit dependency because
> it is a dependency of the robot library.

The following also needs to be added to your `settings.gradle` file:

```gradle
include ':Common'
```
