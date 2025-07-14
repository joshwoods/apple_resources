

- WatchKit
-  Setting up a watchOS project 

# Setting up a watchOS project

Create a new watchOS project or add a watch target to an existing iOS project.

## Overview

Before you start a new watchOS project, you need to decide how you’re going to distribute that project: as a watch-only app, or as a watchOS app with an iOS app. If your app is only available on Apple Watch, create a new watch-only project. If you want a watchOS and iOS app that deliver a related experience, either create a new project that bundles the two apps, or add a watchOS target to an existing iOS project.

### Create a new project

To create a new watchOS project:

1.  In Xcode, choose File \> New \> Project.

2.  Select the watchOS tab.

3.  To create a watch-only app, select “App” and click Next. To create a watchOS app bundled with an iOS app, select “iOS App with Watch App” and click Next.

4.  In the project options sheet (Figure 1), enter a product name for the project. If you plan to implement a custom notification, complication, or unit tests, select the appropriate checkboxes, and click Next.

5.  Select a location for the project, and click Create.

Xcode includes the Notification Scene by default. Leave this checkbox selected even if you don’t plan on implementing notifications right away. Selecting the checkbox adds the `PushNotificationPayload.apns` file to your project, which helps you debug your notification interfaces. If you add a Notification Scene later, you must also add the `PushNotificationPayload.apns` file.

### Add a watchOS app target to an existing iOS project

You can add a watchOS target to an existing iOS project by following these steps:

1.  Open your iOS app’s project in Xcode.

2.  Choose File \> New \> Target.

3.  Select the watchOS tab.

4.  Select “Watch App for iOS App” and click Next.

5.  In the target options sheet (Figure 2), enter a Product Name for the project. If you plan to implement notifications or complications, select the appropriate checkboxes, and click Finish.

6.  Xcode then asks you to activate the new scheme for your watch target. Click Activate.

As when creating a new project, Xcode includes the Notification Scene by default. Leave this checkbox selected even if you don’t plan to implement notifications right away; selecting the checkbox adds the `PushNotificationPayload.apns` file to your project, which helps you debug your notification interfaces. If you add a Notification Scene later, you must also add the `PushNotificationPayload.apns` file.

### Understand the WatchKit app and WatchKit extension

Regardless of whether you add a watchOS app to an existing project or create a new project that contains both an iOS and watchOS app, Xcode automatically configures the targets for your watchOS app and adds the needed files, as in Figure 3.

Xcode divides the watchOS app into two sections:

WatchKit App  
An app bundle that contains your watchOS app’s storyboard and any assets used by the storyboard.

WatchKit Extension  
An extension that contains your watchOS app’s code.

Xcode sets the bundle IDs for both of the watch targets based on the container’s ID. For a watch-only app, this ID is the bundle ID for the root target. For a watchOS app with an iOS app, this ID is the iOS app’s bundle ID. The root of the WatchKit app and WatchKit extension’s bundle IDs must match the container’s bundle ID. If you change your iOS app’s bundle ID, you must update the other bundle IDs accordingly.

When developing your watchOS app, edit your app’s storyboard in the WatchKit app, and write your app’s code in the WatchKit extension. Your WatchKit extension connects to controls and views in the storyboard using WKInterfaceObject subclasses such as WKInterfaceButton and WKInterfaceLabel. These interface objects act as proxies for your storyboard elements. Use the interface elements to configure the elements in code.

## Topics

### Information Property List Keys

The keys that Xcode automatically sets in the information property list file when you create a watchOS target.

WKWatchKitApp

A Boolean value that indicates whether the bundle is a watchOS app.

WKAppBundleIdentifier

The bundle ID of the watchOS app.

WKCompanionAppBundleIdentifier

The bundle ID of the watchOS app’s companion iOS app.

WKExtensionDelegateClassName

The name of your watchOS app’s extension delegate.

WKRunsIndependentlyOfCompanionApp

A Boolean value indicating whether the user can install and run the watchOS app independently of its iOS companion app.

WKWatchOnly

A Boolean value indicating whether the app is a watch-only app.

## See Also

### App structure

class WKApplication

The centralized point of control and coordination for apps with a single watchOS app target.

protocol WKApplicationDelegate

A collection of methods that manages the app-level behavior for a single-target watchOS app.

class WKExtension

The centralized point of control and coordination for extension-based apps running in watchOS.

protocol WKExtensionDelegate

A collection of methods that manages the app-level behavior of a WatchKit extension.

func WKApplicationMain(Int32, UnsafeMutablePointer&lt;UnsafeMutablePointer&lt;CChar>?>, String?) -> Int32

Creates the application object and the application delegate, and sets up the app’s event cycle.

class WKInterfaceDevice

An object that provides information about the user’s Apple Watch.

WKPrefersNetworkUponForeground

A Boolean value that indicates whether an app requires network access on launch.

