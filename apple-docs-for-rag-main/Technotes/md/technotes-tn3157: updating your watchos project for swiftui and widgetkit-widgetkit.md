

- Technotes
-  TN3157: Updating your watchOS project for SwiftUI and WidgetKit 

Article

# TN3157: Updating your watchOS project for SwiftUI and WidgetKit

Update your watchOS app project to adopt SwiftUI, WidgetKit, and other modern features.

## Overview

Since the debut of Apple Watch, watchOS app development has the following important milestones:

- In 2015, watchOS 1 was released, together with WatchKit and ClockKit.

- In 2020, watchOS 7 was released. WatchKit storyboards were deprecated. New developments use SwiftUI.

- In 2022, Xcode 14 was released. It removes the support of creating a new WatchKit storyboard, and introduces single-target watchOS app.

- In 2023, watchOS 10 was released. ClockKit complications were deprecated, and the replacement is WidgetKit complications.

SwiftUI is cross-platform and provides many features unavailable in WatchKit, such as TimelineView and TabView. WidgetKit complications support Smart Stack in watchOS 10. Making a watchOS app single-target simplifies the project configuration. If you have an existing watchOS app, now is the time to get rid of the deprecated WatchKit storyboards and ClockKit complications, and adopt the modern features.

## The terminology

This technote uses the following terminology to refer a watchOS app with different characteristics:

- A **dependent** app relies on its companion iOS app to function.

- An **independent** app works when the paired iPhone isn’t nearby, or when its companion iOS app isn’t installed. It may or may not have a companion iOS app.

- A **dual-target** app has a watchOS app target and a WatchKit extension target for its core functionality.

- A **single-target** app has only a watchOS app target for its core functionality.

- A **watch-only** app doesn’t have a companion iOS app.

Note

Both single-target and dual-target apps can have other targets. For example, you can add targets to implement widgets or app intents for a single-target or dual-target app.

## From dependent to independent

Apple Watch users expect that the apps to just work, even when they don’t have their iPhones with them. If you have a dependent watchOS app, consider making it independent. See Creating independent watchOS apps for details.

## From dual-target to single-target

If your watchOS app is dual-target, convert it to single-target. This simplifies the project configuration and eliminates any confusion about where to embed a resource or apply an entitlement. Single-target watchOS apps work on watchOS 7 and later. For more information, see Build a productivity app for Apple Watch.

Note

A single-target watchOS app requires watchOS 9.2 or later to inherit the HealthKit permissions granted to its companion iOS app. If your app uses HealthKit and needs to support earlier versions of watchOS, keep your dual-target app configuration.

To convert a dual-target app to a single target:

1.  Create a complete back up for your project so you can roll back if something goes wrong.

2.  In Xcode’s Project navigator, select the project, then choose Xcode \> Editor \> Validate Settings.

3.  Select the “Project - Upgrade to a single-target watch app” checkbox if unselected, then choose Perform Changes to let Xcode do the conversion.

4.  If you use storyboards, go through all the interface controllers, and change the class module to the watchOS app module. To do that, select an interface control, and choose View \> Inspectors \> Identity; in the inspector, set the Class field in the Custom Class section.

5.  Remove the files only relevant to the WatchKit extension, such as the extension’s `Info.plist`.

6.  Clean up your project by re-organizing the groups and files in Xcode’s Project navigator.

The second step removes the WatchKit extension target and moves its associated source code and resources to the watchOS app target. At the code level, it replaces WKExtension and WKExtensionDelegate with WKApplication and WKApplicationDelegate. It also changes the `Info.plist` of the watchOS app target as needed. For example, if your watchOS app has a complication, it moves the complication controller class, which is specified with CLKComplicationPrincipalClass, to the watchOS app target, and adds the `CLKComplicationPrincipalClass` and CLKComplicationSupportedFamilies entries to the watchOS app’s `Info.plist`.

You now have a single-target watchOS app project. Verify that everything works well by running the project on an Apple Watch.

## From WatchKit storyboards to SwiftUI

To adopt SwiftUI lifecycle in your watchOS app, start by adding a SwiftUI app (App) struct:

```
import SwiftUI

@main
struct MyWatchApp: App {
    var body: some Scene {
        WindowGroup {
            Text("Hello, world!")
        }
    }
}
```

If you need to run the `WKApplicationDelegate` methods in the SwiftUI lifecycle, use WKApplicationDelegateAdaptor to connect the app delegate to the SwiftUI app. Otherwise, remove the delegate class.

```
import WatchKit
import SwiftUI

//@main
class MyWatchAppDelegate: NSObject, WKApplicationDelegate {...}

@main
struct MyWatchApp: App {
    @WKApplicationDelegateAdaptor var appDelegate: MyWatchAppDelegate
    var body: some Scene {...}
}
```

If you still use WKExtensionDelegate and need to run the extension delegate methods in the SwiftUI lifecycle, migrate `WKExtensionDelegate` to `WKApplicationDelegate`.

To migrate your WatchKit storyboard, rewrite the interface with SwiftUI. Alternatively, consider adopting SwiftUI incrementally by using WKHostingController to host SwiftUI views in your WatchKit interface controllers.

## From ClockKit to WidgetKit complications

To migrate a ClockKit complication to WidgetKit:

1.  Create a widget to replace the ClockKit complication. See Creating accessory widgets and watch complications for details.

2.  Implement CLKComplicationWidgetMigrator in the complication controller class to migrate the ClockKit complication. See Migrating ClockKit complications to WidgetKit for details.

Note

When the ClockKit complication doesn’t have a descriptor, the system passes a descriptor with the default identifier (CLKDefaultComplicationIdentifier) to getWidgetConfiguration(from:completionHandler:). Ignore the descriptor and return a CLKComplicationWidgetMigrationConfiguration object with the appropriate widget kind.

## From a watch-only app to a watchOS app with a companion iOS app

SwiftUI and WidgetKit are both cross-platform. If you have a watch-only app, you might want to enhance the watchOS app by adding an iOS companion app, and have the iOS app share SwiftUI views and widgets with the watchOS app.

Note

After adding an iOS companion app and publishing it to the App Store, you can’t roll back to a watch-only app.

To add an iOS companion app to an existing watch-only app project:

1.  Create a complete back up for your project so you can roll back if something goes wrong.

2.  In Xcode, select your project in the Project navigator, then add a new iOS app target.

3.  Select the iOS app target from the Targets list, click the Signing & Capabilities tab, then choose a team from the Team pop-up menu and enter a bundle ID. Be sure that the iOS app’s bundle ID is the prefix of the watchOS app’s bundle ID. For example, if the watchOS app’s bundle ID is `com.YourCompany.ProductName.watchkitapp`, the iOS app’s bundle ID must be `com.YourCompany.ProductName`.

4.  Select the General tab, then under Frameworks, Libraries, and Embedded Content, add the watchOS app as an embedded content of the iOS app.

5.  Confirm that the WKCompanionAppBundleIdentifier key in the watchOS app’s `Info.plist` is set to the bundle ID of the iOS app.

You now have a project that has an independent watchOS app with a companion iOS app. By default, Xcode doesn’t install the iOS app when running the watchOS app. If you’d like to change the behavior, add the WKRunsIndependentlyOfCompanionApp entry to the `Info.plist` of the watchOS app, then set its value to `NO`.

## Revision History

- **2023-11-07** First published.

## See Also

### Latest

TN3182: Adding privacy tracking keys to your privacy manifest

Declare the tracking domains you use in your app or third-party SDK in a privacy manifest.

TN3183: Adding required reason API entries to your privacy manifest

Declare the APIs that can potentially fingerprint devices in your app or third-party SDK in a privacy manifest.

TN3184: Adding data collection details to your privacy manifest

Declare the data your app or third-party SDK collects in a privacy manifest.

TN3181: Debugging an invalid privacy manifest

Identify common configurations that cause unsuccessful privacy manifest validation with the App Store.

TN3180: Reverting to App Store Server Notifications V1

Migrate from version 2 to version 1 of App Store Server Notifications using the Modify an App endpoint.

TN3179: Understanding local network privacy

Learn how local network privacy affects your software.

TN3178: Checking for and resolving build UUID problems

Ensure that every Mach-O image has a UUID, and that every distinct Mach-O image has its own unique UUID.

TN3177: Understanding alternate audio track groups in movie files

Learn how alternate groups collect audio tracks, and how to choose which audio track to use in your app.

TN3111: iOS Wi-Fi API overview

Explore the various Wi-Fi APIs available on iOS and their expected use cases.

TN3176: Troubleshooting Apple Pay payment processing issues

Diagnose errors that occur when processing Apple Pay payments, identify common causes, and explore potential solutions.

TN3175: Diagnosing issues with displaying the Apple Pay button on your website

Diagnose common errors received while displaying the Apple Pay button on your website by identifying the underlying causes, and explore potential solutions.

TN3174: Diagnosing issues with the Apple Pay payment sheet on your website

Diagnose errors received while presenting the Apple Pay payment sheet on your website by identifying the underlying causes of common errors and explore their potential solutions.

TN3173: Troubleshooting issues with your Apple Pay merchant identifier configuration

Diagnose errors due to invalid Apple Pay merchant identifier configurations by identifying the underlying causes of common errors and explore their potential solutions.

TN3168: Making your App Clip available in the App Store

Learn how to configure your App Clip to prevent it from being unavailable in the App Store.

TN3124: Debugging coordinate space issues

Learn techniques to help debug any coordinate space issue.

