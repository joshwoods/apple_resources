

- SwiftUI
-  WKExtensionDelegateAdaptor 

Structure

# WKExtensionDelegateAdaptor

A property wrapper type that you use to create a WatchKit extension delegate.

watchOS 7.0+

``` source
@MainActor @preconcurrency @propertyWrapper
struct WKExtensionDelegateAdaptor where DelegateType : NSObject, DelegateType : WKExtensionDelegate
```

## Overview

To handle extension delegate callbacks in an extension that uses the SwiftUI life cycle, define a type that conforms to the WKExtensionDelegate protocol, and implement the delegate methods that you need. For example, you can implement the didRegisterForRemoteNotifications(withDeviceToken:) method to handle remote notification registration:

```
class MyExtensionDelegate: NSObject, WKExtensionDelegate, ObservableObject {
    func didRegisterForRemoteNotifications(withDeviceToken: Data) {
        // Record the device token.
    }
}
```

Then use the `WKExtensionDelegateAdaptor` property wrapper inside your App declaration to tell SwiftUI about the delegate type:

```
@main
struct MyApp: App {
    @WKExtensionDelegateAdaptor private var extensionDelegate: MyExtensionDelegate

    var body: some Scene { ... }
}
```

SwiftUI instantiates the delegate and calls the delegate’s methods in response to life cycle events. Define the delegate adaptor only in your App declaration, and only once for a given extension. If you declare it more than once, SwiftUI generates a runtime error.

If your extension delegate conforms to the ObservableObject protocol, as in the example above, then SwiftUI puts the delegate it creates into the Environment. You can access the delegate from any scene or view in your extension using the EnvironmentObject property wrapper:

```
@EnvironmentObject private var extensionDelegate: MyExtensionDelegate
```

This enables you to use the dollar sign (`$`) prefix to get a binding to published properties that you declare in the delegate. For more information, see projectedValue.

Important

Manage an externsion’s life cycle events without using a delegate whenever possible. For example, prefer to handle changes in ScenePhase instead of relying on delegate callbacks, like applicationDidFinishLaunching().

## Topics

### Creating a delegate adaptor

init(_:)

Creates a WatchKit extension delegate adaptor using an observable delegate.

### Getting the delegate adaptor

var projectedValue: ObservedObject&lt;DelegateType>.Wrapper

A projection of the observed object that provides bindings to its properties.

var wrappedValue: DelegateType

The underlying delegate.

## Relationships

### Conforms To

- DynamicProperty
- Sendable

## See Also

### Targeting watchOS

struct WKApplicationDelegateAdaptor

A property wrapper that is used in `App` to provide a delegate from WatchKit.

