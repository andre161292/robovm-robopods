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

compile "org.robovm:robopods-google-apis-ios:1.6.0"
compile "org.robovm:robopods-google-instance-id-ios:1.6.0"
compile "org.robovm:robopods-google-cloud-messaging-ios:1.6.0"

Possible issues:

    CocoaPods libraries (.a) are committed in robopods/META-INF/robovm/ios/libs directories. I don't think there is any licensing issues, but it's better to double check this point.
    libGTM_AddressBook.a in GoogleUtilities gives link errors with my project (undefined symbols). It doesn't seem to be used by cloud messaging, so I have simply commented out the lib reference in the robovm.xml file (see comments in robovm.xml).
