# Power_Play
EOCV-AprilTag-Plugin
A plug and play module for detecting AprilTags on an FTC robot, designed to be used from EasyOpenCV

Installation instructions:
IMPORTANT NOTE: This assumes you have already installed EasyOpenCV!

Open your FTC SDK Android Studio project

Open the build.gradle file for the TeamCode module:

At the bottom, add this:

 dependencies {
     implementation 'org.openftc:apriltag:1.1.0'
  }
Now perform a Gradle Sync:

img-here

Congrats, you're ready to go! Now check out the example OpModes and pipeline in the examples directory.

AprilTag images
You can download a PDF with the first 20 tags of the 36h11 family here

Alternatively, you can find PNGs here

Changelog:
v1.1.0
Updates to latest version of AprilTag as of 30 March 2022
Fixes small memory leak for frames where no detections were found
Protects against NULL pointers in native JNI code
Updates AprilTagDetectionPipeline to create the native detector in the constructor instead of in init(). NOTE: You will need to copy-paste the updated file, as this file is not part of the binary release!
v1.0.0
Initial release
