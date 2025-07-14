

- UIKit
-  UIWindowSceneDelegate 

Protocol

# UIWindowSceneDelegate

Additional methods that you use to manage app-specific tasks occurring in a scene.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+tvOS 13.0+visionOS 1.0+

``` source
@MainActor
protocol UIWindowSceneDelegate : UISceneDelegate
```

## Mentioned in 

Specifying the scenes your app supports

## Overview

Use your UIWindowSceneDelegate object to manage the life cycle of one instance of your app’s user interface. The window scene delegate conforms to the UISceneDelegate protocol, and you use it to receive notifications when its scene connects to the app, enters the foreground, and so on. You also use it to respond to changes in the underlying environment of the scene. For example, if the user resizes a scene, use your delegate to make any needed changes to your content to accommodate the new size.

Don’t create UIWindowSceneDelegate objects directly. Instead, specify the name of your delegate class as part of the configuration data for your scene. You can specify this information in your app’s `Info.plist` file, or in the UISceneConfiguration object you return from your app delegate’s application(_:configurationForConnecting:options:) method. For more information about how to configure scenes, see Specifying the scenes your app supports.

For an example on using `UIWindowSceneDelegate` in your app, see Supporting multiple windows on iPad.

## Topics

### Managing the scene’s main window

var window: UIWindow?

The main window associated with the scene.

### Responding to scene changes

func windowScene(UIWindowScene, didUpdate: any UICoordinateSpace, interfaceOrientation: UIInterfaceOrientation, traitCollection: UITraitCollection)

Notifies you when the size, orientation, or traits of a scene change.

### Performing tasks

func windowScene(UIWindowScene, performActionFor: UIApplicationShortcutItem, completionHandler: (Bool) -> Void)

Asks the delegate to perform the user-selected action.

func windowScene(UIWindowScene, userDidAcceptCloudKitShareWith: CKShareMetadata)

Tells the delegate that the window scene now has access to shared information in CloudKit.

## Relationships

### Inherits From

- NSObjectProtocol
- UISceneDelegate

## See Also

### Window scenes

Supporting multiple windows on iPad

Support side-by-side instances of your app’s interface and create new windows.

class UIWindowScene

A scene that manages one or more windows for your app.

class UIScene

An object that represents one instance of your app’s user interface.

protocol UISceneDelegate

The core methods you use to respond to life-cycle events occurring within a scene.

