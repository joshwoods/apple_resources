

- SwiftUI
-  UIApplicationDelegateAdaptor 

Structure

# UIApplicationDelegateAdaptor

A property wrapper type that you use to create a UIKit app delegate.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+tvOS 14.0+visionOS 1.0+

``` source
@MainActor @preconcurrency @propertyWrapper
struct UIApplicationDelegateAdaptor where DelegateType : NSObject, DelegateType : UIApplicationDelegate
```

## Mentioned in 

Migrating to the SwiftUI life cycle

## Overview

To handle app delegate callbacks in an app that uses the SwiftUI life cycle, define a type that conforms to the UIApplicationDelegate protocol, and implement the delegate methods that you need. For example, you can implement the application(_:didRegisterForRemoteNotificationsWithDeviceToken:) method to handle remote notification registration:

```
class MyAppDelegate: NSObject, UIApplicationDelegate, ObservableObject {
    func application(
        _ application: UIApplication,
        didRegisterForRemoteNotificationsWithDeviceToken deviceToken: Data
    ) {
        // Record the device token.
    }
}
```

Then use the `UIApplicationDelegateAdaptor` property wrapper inside your App declaration to tell SwiftUI about the delegate type:

```
@main
struct MyApp: App {
    @UIApplicationDelegateAdaptor private var appDelegate: MyAppDelegate

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

Manage an app’s life cycle events without using an app delegate whenever possible. For example, prefer to handle changes in ScenePhase instead of relying on delegate callbacks, like application(_:didFinishLaunchingWithOptions:).

### Scene delegates

Some iOS apps define a UIWindowSceneDelegate to handle scene-based events, like app shortcuts:

```
class MySceneDelegate: NSObject, UIWindowSceneDelegate, ObservableObject {
    func windowScene(
        _ windowScene: UIWindowScene,
        performActionFor shortcutItem: UIApplicationShortcutItem
    ) async -> Bool {
        // Do something with the shortcut...

        return true
    }
}
```

You can provide this kind of delegate to a SwiftUI app by returning the scene delegate’s type from the application(_:configurationForConnecting:options:) method inside your app delegate:

```
extension MyAppDelegate {
    func application(
        _ application: UIApplication,
        configurationForConnecting connectingSceneSession: UISceneSession,
        options: UIScene.ConnectionOptions
    ) -> UISceneConfiguration {

        let configuration = UISceneConfiguration(
                                name: nil,
                                sessionRole: connectingSceneSession.role)
        if connectingSceneSession.role == .windowApplication {
            configuration.delegateClass = MySceneDelegate.self
        }
        return configuration
    }
}
```

When you configure the UISceneConfiguration instance, you only need to indicate the delegate class, and not a scene class or storyboard. SwiftUI creates and manages the delegate instance, and sends it any relevant delegate callbacks.

As with the app delegate, if you make your scene delegate an observable object, SwiftUI automatically puts it in the Environment, from where you can access it with the EnvironmentObject property wrapper, and create bindings to its published properties.

## Topics

### Creating a delegate adaptor

init(_:)

Creates a UIKit app delegate adaptor using an observable delegate.

### Getting the delegate adaptor

var projectedValue: ObservedObject&lt;DelegateType>.Wrapper

A projection of the observed object that provides bindings to its properties.

var wrappedValue: DelegateType

The underlying app delegate.

## Relationships

### Conforms To

- DynamicProperty
- Sendable

## See Also

### Targeting iOS and iPadOS

UILaunchScreen

The user interface to show while an app launches.

UILaunchScreens

The user interfaces to show while an app launches in response to different URL schemes.

