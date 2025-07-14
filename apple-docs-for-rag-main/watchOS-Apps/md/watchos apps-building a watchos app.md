

- watchOS apps
-  Building a watchOS app 

Article

# Building a watchOS app

Set up your app’s life cycle and create its user interface with SwiftUI.

## Overview

Develop powerful, personal apps for Apple Watch using SwiftUI, a declarative framework for building user interfaces on all of Apple’s platforms. You can create rich user interfaces by composing simple views — which perform a single, focused task — into larger, more complex layouts. Your app describes the correct layout for its views based on its current state. SwiftUI detects changes to the state and updates the views accordingly.

On watchOS, SwiftUI gives you considerably more freedom, power, and control than user interfaces laid out and designed in a storyboard. For example, List has a number of features that aren’t supported by WKInterfaceTable, such as the platter style, swipe actions (shown below), and row reordering.

Additionally, you can preview your SwiftUI code in Xcode’s canvas. You can design, build, and test your interfaces without ever running your app.

SwiftUI also provides watch-specific representations of tab and navigation views, with fully customizable navigation bars and customizable toolbar items for confirmation, cancellation, and destructive actions. You can also use SwiftUI to manage your app’s life cycle. To learn more about SwiftUI, see Introducing SwiftUI.

### Set up the root view

To manage your app’s life cycle with SwiftUI, create a structure that adopts the App protocol in your watchOS app target.

```
import SwiftUI

@main
struct MyProject_Watch_App: App {
}
```

The @main attribute indicates this is the entry point for your app. Each app can have only one entry point.

Inside the structure, define the app’s body. The `body` automatically composes a collection of Scene instances into a single, compound `Scene`.

```
@main
struct MyProject_Watch_App: App {
    var body: some Scene {
    }
}
```

Next, add a `Scene` or your app’s root view. For a watchOS app, you typically create a WindowGroup scene that wraps a NavigationView around your app’s root view. The `NavigationView` provides a navigation stack and title area for your app.

```
@main
struct MyProject_Watch_App: App {
    var body: some Scene {
        WindowGroup {
            NavigationView {
                ContentView()
            }
        }
    }
}
```

When your app launches, it displays the view hierarchy defined by the window group.

You can also add scenes for notification categories.

```
var body: some Scene {
    WindowGroup {
        NavigationView {
            ContentView()
        }
    }

    WKNotificationScene(controller: NotificationController.self, category: "myCategory")
}
```

When the system receives a notification with a matching category, it displays a dynamic view specified by the notification controller. You can create a WKUserNotificationHostingController subclass for each notification category supported by your app.

```
import SwiftUI
import UserNotifications

class NotificationController: WKUserNotificationHostingController {

    var content:UNNotificationContent!
    var date:Date!

    override var body: NotificationLongLook{
        NotificationLongLook(content: content, date: date)
    }

    override class var isInteractive: Bool { true }

    override func didReceive(_ notification: UNNotification) {
        content = notification.request.content
        date = notification.date
    }
}
```

For more information, see Customizing your long-look interface.

### Respond to app events in SwiftUI

Your app can respond to many app events directly in SwiftUI.

SwiftUI updates the scenePhase environment value as your app changes state. To update a view based on these changes, you can use the onChange(of:perform:) modifier. For more information, see Handling Common State Transitions.

SwiftUI also provides view modifiers for handling user activity and background tasks:

- Use onContinueUserActivity(_:perform:) to handle incoming NSUserActivity objects. For more information, see Handling User Activity.

- Use backgroundTask(_:action:) to handle incoming BackgroundTask instances. For more information, see Using background tasks.

### Respond to app events using an app delegate

You need an app delegate to handle the following events:

- Life cycle events, like applicationDidFinishLaunching(), that aren’t handled by the scenePhase environment variable

- `userInfo` dictionaries from either handoff or complications

- Remote Now Playing activity

- Workout configurations and recovery

- Extended runtime sessions

- Registration of remote notifications

To add an app delegate to your app, create a class that adopts the WKApplicationDelegate protocol. In this class, implement the methods needed to handle your app’s events. Then use the WKApplicationDelegateAdaptor property wrapper to declare a variable for your delegate.

```
import SwiftUI
import WatchKit

@main
struct MyProject_Watch_App: App {

    @WKApplicationDelegateAdaptor var appDelegate: MyAppDelegate

    var body: some Scene {
        WindowGroup {
            NavigationView {
                ContentView()
            }
        }

        WKNotificationScene(controller: NotificationController.self, category: "myCategory")
    }
}
```

When your app launches, the system instantiates your delegate class and calls applicationDidFinishLaunching(). Use this method to perform any additional configuration that your delegate requires. After it returns, the system begins calling your delegate methods when the corresponding events occur.

## See Also

### Related Documentation

Creating a watchOS app

This tutorial gives you a chance to apply much of what you’ve already learned about SwiftUI, and — with little effort — migrate the Landmarks app to watchOS.

Life cycles

Receive and respond to life-cycle notifications.

### Essentials

Creating an intuitive and effective UI in watchOS 10

Provide an even more streamlined, consistent, and glanceable user experience with new design features.

Updating your app and widgets for watchOS 10

Integrate SwiftUI elements and watch-specific features, and build widgets for the Smart Stack.

watchOS updates

Learn about important changes to watchOS.

