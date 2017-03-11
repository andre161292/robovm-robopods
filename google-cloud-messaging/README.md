# RoboPods for Google APIs



## Available RoboPods

| Platform    | Version |
|-------------|---------|
| [iOS](ios/) |         |
|             |         |

## Official website

This a complete port of GGLInstanceID and GoogleCloudMessaging from CocoaPods, with their dependencies: GoogleSymbolUtilities, GoogleUtilities, GoogleInterchangeUtilities and GoogleNetworkingUtilities.

It is not yet thoroughly tested but I've used it successfully in a iOS 7+ project with RoboVM (following the instructions given in Setting up a GCM Client App on iOS).

A typical setup requires to add these Gradle dependencies to your ios project:

buildscript {
   project.ext.robopodsVersion = "2.2.1"
}

compile "com.mobidevelop.robovm:robopods-google-apis-ios:$robopodsVersion"

compile "com.mobidevelop.robovm:robopods-google-instance-ido-is:$robopodsVersion"

