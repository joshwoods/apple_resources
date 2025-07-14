

- SwiftUI
-  NSApplicationDelegateAdaptor 

Structure

# NSApplicationDelegateAdaptor

A property wrapper type that you use to create an AppKit app delegate.

macOS 11.0+

``` source
@MainActor @preconcurrency @propertyWrapper
struct NSApplicationDelegateAdaptor where DelegateType : NSObject, DelegateType : NSApplicationDelegate
```

## Mentioned in 

Migrating to the SwiftUI life cycle

## Overview

To handle app delegate callbacks in an app that uses the SwiftUI life cycle, define a type that conforms to the NSApplicationDelegate protocol, and implement the delegate methods that you need. For example, you can implement the application(_:didRegisterForRemoteNotificationsWithDeviceToken:) method to handle remote notification registration:

```
class MyAppDelegate: NSObject, NSApplicationDelegate, ObservableObject {
    func application(
        _ application: NSApplication,
        didRegisterForRemoteNotificationsWithDeviceToken deviceToken: Data
    ) {
        // Record the device token.
    }
}
```

Then use the `NSApplicationDelegateAdaptor` property wrapper inside your App declaration to tell SwiftUI about the delegate type:

```
@main
struct MyApp: App {
    @NSApplicationDelegateAdaptor private var appDelegate: MyAppDelegate

    var body: some Scene { ... }
}
```

SwiftUI instantiates the delegate and calls the delegate’s methods in response to life cycle events. Define the delegate adaptor only in your App declaration, and only once for a given app. If you declare it more than once, SwiftUI generates a runtime error.

If your app delegate conforms to the ObservableObject protocol, as in the example above, then SwiftUI puts the delegate it creates into the Environment. You can access the delegate from any scene or view in your app using the EnvironmentObject property wrapper:

```
@EnvironmentObject private var appDelegate: MyAppDelegate
```

This enables you to use the dollar sign (`$`) prefix to get a binding to published properties that you declare in the delegate. For more information, see projectedValue.

Important

Manage an app’s life cycle events without using an app delegate whenever possible. For example, prefer to handle changes in ScenePhase instead of relying on delegate callbacks, like applicationDidFinishLaunching(_:).

## Topics

### Creating a delegate adaptor

init(_:)

Creates an AppKit app delegate adaptor using an observable delegate.

### Getting the delegate adaptor

var projectedValue: ObservedObject&lt;DelegateType>.Wrapper

A projection of the observed object that provides bindings to its properties.

var wrappedValue: DelegateType

The underlying delegate.

## Relationships

### Conforms To

- DynamicProperty
- Sendable

