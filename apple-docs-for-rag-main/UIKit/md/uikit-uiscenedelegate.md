

- UIKit
-  UISceneDelegate 

Protocol

# UISceneDelegate

The core methods you use to respond to life-cycle events occurring within a scene.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+tvOS 13.0+visionOS 1.0+

``` source
@MainActor
protocol UISceneDelegate : NSObjectProtocol
```

## Overview

Use your UISceneDelegate object to manage life-cycle events in one instance of your app’s user interface. This interface defines methods for responding to state transitions that affect the scene, including when the scene enters the foreground and becomes active, and when it enters the background. Use your delegate to provide appropriate behavior when these transitions occur. For example, finish critical tasks and quiet your app when it enters the background.

Don’t create UISceneDelegate objects directly. Instead, specify the name of your custom delegate class as part of the configuration data for your scenes. You can specify this information in your app’s `Info.plist` file, or in the UISceneConfiguration object you return from your app delegate’s application(_:configurationForConnecting:options:) method. For more information about how to configure scenes, see Specifying the scenes your app supports.

## Topics

### Working with window scenes

Supporting multiple windows on iPad

Support side-by-side instances of your app’s interface and create new windows.

### Connecting and disconnecting the scene

func scene(UIScene, willConnectTo: UISceneSession, options: UIScene.ConnectionOptions)

Tells the delegate about the addition of a scene to the app.

func sceneDidDisconnect(UIScene)

Tells the delegate that UIKit removed a scene from your app.

class ConnectionOptions

A data object containing information about the reasons why UIKit created the scene.

### Transitioning to the foreground

func sceneWillEnterForeground(UIScene)

Tells the delegate that the scene is about to begin running in the foreground and become visible to the user.

func sceneDidBecomeActive(UIScene)

Tells the delegate that the scene became active and is now responding to user events.

### Transitioning to the background

func sceneWillResignActive(UIScene)

Tells the delegate that the scene is about to resign the active state and stop responding to user events.

func sceneDidEnterBackground(UIScene)

Tells the delegate that the scene is running in the background and is no longer onscreen.

### Opening URLs

func scene(UIScene, openURLContexts: Set&lt;UIOpenURLContext>)

Asks the delegate to open one or more URLs.

### Continuing user activities

func scene(UIScene, willContinueUserActivityWithType: String)

Tells the delegate that it’s about to receive Handoff-related data.

func scene(UIScene, continue: NSUserActivity)

Tells the delegate to handle the specified Handoff-related activity.

func scene(UIScene, didFailToContinueUserActivityWithType: String, error: any Error)

Tells the delegate that the activity couldn’t be continued.

### Saving the state of the scene

Restoring your app’s state

Provide continuity for the user by preserving current activities.

func stateRestorationActivity(for: UIScene) -> NSUserActivity?

Returns a user activity object encapsulating the current state of the specified scene.

func scene(UIScene, restoreInteractionStateWith: NSUserActivity)

func scene(UIScene, didUpdate: NSUserActivity)

Tells the delegate that the specified activity object was updated.

## Relationships

### Inherits From

- NSObjectProtocol

### Inherited By

- UIWindowSceneDelegate

## See Also

### Window scenes

Supporting multiple windows on iPad

Support side-by-side instances of your app’s interface and create new windows.

protocol UIWindowSceneDelegate

Additional methods that you use to manage app-specific tasks occurring in a scene.

class UIWindowScene

A scene that manages one or more windows for your app.

class UIScene

An object that represents one instance of your app’s user interface.

