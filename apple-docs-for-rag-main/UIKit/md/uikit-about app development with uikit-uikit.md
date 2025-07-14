

- UIKit
-  About App Development with UIKit 

Article

# About App Development with UIKit

Learn about the basic support that UIKit and Xcode provide for your iOS and tvOS apps.

## Overview

The UIKit framework provides the core objects that you need to build apps for iOS and tvOS. You use these objects to display your content onscreen, to interact with that content, and to manage interactions with the system. Apps rely on UIKit for their basic behavior, and UIKit provides many ways for you to customize that behavior to match your specific needs.

Important

You always start the development of an iOS or tvOS app by creating a project in Xcode, Apple’s integrated development environment. If you don’t have Xcode, you can download it from the App Store. You can also download the latest version from developer.apple.com.

Xcode provides template projects as starting points for every app you create. For example, the following image shows the structure of an app created using the single view app template in Xcode. The template projects provide a minimal user interface, so you can build and run your project immediately and see the results on a device or in the simulator.

When you build your app, Xcode compiles your source files and creates an app bundle for your project. An app bundle is a structured directory that contains the code and resources associated with the app. Resources include the image assets, storyboard files, strings files, and app metadata that support your code. The structure of the app bundle is important, but Xcode knows where your resources need to go, so don’t worry about it for now.

### Required Resources

Every UIKit app is required to have the following resources:

- App icons

- Launch screen storyboard

The system displays your app icon on the Home screen, in Settings, and anywhere it needs to differentiate your app from other apps. Because it is used in multiple places, and on multiple devices, you provide multiple versions of your app icon in your Xcode project’s AppIcon image asset. Your app icon should be distinctive to help the user identify your app quickly on the Home screen. However, you may vary the details of your icon to accommodate the different image sizes that you must provide.

The `LaunchScreen.storyboard` file contains your app’s initial user interface, and it can be a splash screen or a simplified version of your actual interface. When the user taps your app’s icon, the system displays your launch screen immediately, letting the user know that your app is now launching. The launch screen also provides cover for your app while it initializes itself. When your app is ready, the system hides the launch screen and reveals your app’s actual interface.

### Required App Metadata

The system derives information about your app’s configuration and capabilities from the information property list (`Info.plist`) file in your app bundle. Xcode provides a preconfigured version of this file with every new project template, but you will likely need to modify this file at some point. For example, if your app relies on specific hardware, or uses specific system frameworks, you might need to add information related to those features to this file.

One common modification you can make to the `Info.plist` file is to declare your app’s hardware and software requirements. These requirements are how you communicate to the system what your app needs to run. For example, a navigation app might require the presence of GPS hardware to provide turn-by-turn directions. The App Store prevents an app from being installed on a device that does not meet your app’s requirements.

For information about the keys that you can include in your `Info.plist` file, see Information Property List Key Reference.

### Code Structure of a UIKit App

UIKit provides many of your app’s core objects, including those that interact with the system, run the app’s main event loop, and display your content onscreen. You use most of these objects as-is or with only minor modifications. Knowing which objects to modify, and when to modify them, is crucial to implementing your app.

The structure of UIKit apps is based on the Model-View-Controller (MVC) design pattern, wherein objects are divided by their purpose. Model objects manage the app’s data and business logic. View objects provide the visual representation of your data. Controller objects act as a bridge between your model and view objects, moving data between them at appropriate times.

The following image represents a fairly typical structure of a UIKit app. You provide the model objects that represent your app’s data structures. UIKit provides most of the view objects, although you can define custom views for your data, as needed. Coordinating the exchange of data between your data objects and the UIKit views are your view controllers and app delegate object.

The UIKit and Foundation frameworks provide many of the basic types that you use to define your app’s model objects. UIKit provides a UIDocument object for organizing the data structures that belong in a disk-based file. The Foundation framework defines basic objects representing strings, numbers, arrays, and other data types. The Swift Standard Library provides many of the same types available in the Foundation framework.

UIKit provides most of the objects in the controller and view layers of your app. Specifically, UIKit defines the UIView class, which is usually responsible for displaying your content onscreen. (You can also render content directly to the screen using Metal and other system frameworks.) The UIApplication object runs your app’s main event loop and manages your app’s overall life cycle.

## See Also

### Essentials

UIKit updates

Learn about important changes to UIKit.

Protecting the User’s Privacy

Secure personal data, and respect user preferences for how data is used.

