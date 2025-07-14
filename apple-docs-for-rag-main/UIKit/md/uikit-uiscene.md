

- UIKit
-  UIScene 

Class

# UIScene

An object that represents one instance of your app’s user interface.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+tvOS 13.0+visionOS 1.0+

``` source
@MainActor
class UIScene
```

## Overview

UIKit creates a scene object for each instance of your app’s UI that the user or your app requests. Typically, UIKit creates a UIWindowScene object instead of a UIScene object, but you use the methods and properties of this class to access information about a scene.

Every scene object has an associated delegate object, an object that adopts the UISceneDelegate protocol. When the state of the scene changes, the scene object notifies its delegate object and posts appropriate notifications to registered observer objects. Use the delegate object and notifications to respond to changes in the state of the scene. For example, use it to determine when your scene moves to the background.

You don’t create scene objects directly. You can programmatically ask UIKit to create a scene object for your app by calling the requestSceneSessionActivation(_:userActivity:options:errorHandler:) method of UIApplication. UIKit also creates scenes in response to user interactions. When configuring your app’s scene support, specify UIWindowScene objects instead of UIScene objects.

## Topics

### Creating a scene object

init(session: UISceneSession, connectionOptions: UIScene.ConnectionOptions)

Creates a scene object using the specified session and connection information.

### Managing the life cycle of a scene

var delegate: (any UISceneDelegate)?

The object you use to receive life-cycle events associated with the scene.

protocol UISceneDelegate

The core methods you use to respond to life-cycle events occurring within a scene.

### Getting the scene attributes

var activationState: UIScene.ActivationState

The current execution state of the scene.

enum ActivationState

Constants that indicate the foreground or background execution state of your app.

var title: String!

A user-visible string you supply to help users differentiate among your app’s scenes.

var subtitle: String

A string that the app displays in the title bar of a window when running in macOS.

### Specifying the scene’s activation conditions

var activationConditions: UISceneActivationConditions

The conditions that define when UIKit activates the scene object.

class UISceneActivationConditions

The set of conditions that define when UIKit activates the current scene.

### Responding to life cycle notifications

class let willConnectNotification: NSNotification.Name

A notification that indicates that UIKit added a scene to your app.

class let didDisconnectNotification: NSNotification.Name

A notification that indicates that UIKit removed a scene from your app.

class let willEnterForegroundNotification: NSNotification.Name

A notification that indicates that a scene is about to begin running in the foreground and become visible to the user.

class let didActivateNotification: NSNotification.Name

A notification that indicates that the scene is now onscreen and responding to user events.

class let willDeactivateNotification: NSNotification.Name

A notification that indicates that the scene is about to resign the active state and stop responding to user events.

class let didEnterBackgroundNotification: NSNotification.Name

A notification that indicates that the scene is running in the background and is no longer onscreen.

### Working with system protection manager

var systemProtectionManager: UIScene.SystemProtectionManager?

The system protection manager associated with this scene.

class SystemProtectionManager

A class that represents the status of system protection for the scene.

class let systemProtectionDidChangeNotification: NSNotification.Name

A notification posted when the system-protection attributes of a scene change.

### Getting the scene’s session

var session: UISceneSession

The session associated with the scene.

class UISceneSession

An object that contains information about one of your app’s scenes.

### Opening URLs

func open(URL, options: UIScene.OpenExternalURLOptions?, completionHandler: ((Bool) -> Void)?)

Attempts to open the resource at the specified URL asynchronously.

class OpenExternalURLOptions

Options you specify when asking a scene to open a URL.

### Supporting state restoration

func completeStateRestoration()

func extendStateRestoration()

### Getting the pointer lock state

var pointerLockState: UIPointerLockState?

The pointer lock state for the scene.

class UIPointerLockState

An object that contains information about a scene’s pointer lock state.

### Constants

class ActivationRequestOptions

An object that contains information you want the system to use when activating the session associated with a scene.

class UISceneDestructionRequestOptions

An object you pass to UIKit to permanently remove a scene and its associated session from your app.

class OpenURLOptions

Options that UIKit provides when asking your app to open a URL.

### Instance Methods

func getDefaultAudioSession(completionHandler: (AVAudioSession?) -> Void)

Retrieves the audio session that contains all sounds that implicitly belong to this scene.

## Relationships

### Inherits From

- UIResponder

### Inherited By

- UIWindowScene

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol
- NSTouchBarProvider
- Sendable
- UIActivityItemsConfigurationProviding
- UIPasteConfigurationSupporting
- UIResponderStandardEditActions
- UIUserActivityRestoring

## See Also

### Window scenes

Supporting multiple windows on iPad

Support side-by-side instances of your app’s interface and create new windows.

protocol UIWindowSceneDelegate

Additional methods that you use to manage app-specific tasks occurring in a scene.

class UIWindowScene

A scene that manages one or more windows for your app.

protocol UISceneDelegate

The core methods you use to respond to life-cycle events occurring within a scene.

