

- UIKit
- Mac Catalyst
-  Creating a Mac version of your iPad app 

Article

# Creating a Mac version of your iPad app

Bring your iPad app to macOS with Mac Catalyst.

## Overview

With Xcode 11 and later, you can create a Mac version of your iPad app using Mac Catalyst. Configuring your app for Mac can take just a click in a checkbox, although you may need more steps, depending on the features and frameworks that your app uses.

Note

For information about designing a Mac version of your iPad app, see Human Interface Guidelines.

### Configure your app for Mac

To add support for Mac, open your Xcode project and select the iOS target that you want to configure. In the General tab, under Deployment Info, select the Mac checkbox. (If your app supports iPhone only, the checkbox is unavailable.)

When you enable Mac support, Xcode adds the App Sandbox Entitlement to your project. Xcode only includes this entitlement in the Mac version of your app, not the iOS version. Xcode also adds My Mac to the list of destinations. Select this destination to run your Mac app from Xcode.

At this point, you may be able to build and run the Mac version of your app. To give it a try, select My Mac as the destination and run your project.

### Go beyond the checkbox

You may find that the Mac version of your app still doesn’t build because:

- Your project includes incompatible frameworks, libraries, or embedded content.

- Your source code references unsupported APIs.

When you enable Mac support, Xcode automatically excludes incompatible frameworks and embedded content where possible for Mac builds of your project. Still, you may need to manually exclude other frameworks or content.

To manually exclude an item, open Frameworks, Libraries, and Embedded Content under the General tab for your iOS target. Then select iOS as the platform setting for the item. This setting excludes the item from the Mac version of your app.

If you have source code referencing APIs unavailable to the Mac version of your app, enclose the code in a compilation conditional block that uses the `targetEnvironment()` (Swift) or `TARGET_OS_MACCATALYST` (Objective-C) platform condition.

- Swift
- Objective-C

```
#if !targetEnvironment(macCatalyst)
// Code to exclude from Mac.
#endif
```

```
#if !TARGET_OS_MACCATALYST
// Code to exclude from Mac.
#endif
```

You can use these same approaches to include a framework and code that are available only in macOS. For a framework, select macOS for the platform setting, and enclose the code with a `#if targetEnvironment(macCatalyst)` (Swift) or `#if TARGET_OS_MACCATALYST` (Objective-C) statement.

### Make your app more like a Mac app

After following these steps, you should be able to run your iPad app on Mac. But before you ship your new app to customers, it needs a few more changes to make it more like a Mac app. To learn more, see Optimizing your iPad app for Mac.

