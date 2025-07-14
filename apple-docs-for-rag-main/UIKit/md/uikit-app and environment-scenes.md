

- UIKit
- App and environment
-  Scenes 

API Collection

# Scenes

Manage multiple instances of your app’s UI simultaneously, and direct resources to the appropriate instance of your UI.

## Overview

UIKit manages each instance of your app’s UI using a UIWindowScene object. A *scene* contains the windows and view controllers for presenting one instance of your UI. Each scene also has a corresponding UIWindowSceneDelegate object, which you use to coordinate interactions between UIKit and your app. Scenes run concurrently with each other, sharing the same memory and app process space. As a result, a single app may have multiple scenes and scene delegate objects active at the same time.

Manage the configuration of new scenes from your UIApplicationDelegate object.

## Topics

### Essentials

Preparing your UI to run in the foreground

Configure your app to appear onscreen.

Preparing your UI to run in the background

Prepare your app to be suspended.

### Window scenes

Supporting multiple windows on iPad

Support side-by-side instances of your app’s interface and create new windows.

protocol UIWindowSceneDelegate

Additional methods that you use to manage app-specific tasks occurring in a scene.

class UIWindowScene

A scene that manages one or more windows for your app.

class UIScene

An object that represents one instance of your app’s user interface.

protocol UISceneDelegate

The core methods you use to respond to life-cycle events occurring within a scene.

### Configuration

Specifying the scenes your app supports

Tell the system about your app’s scenes, including the objects you use to manage each scene and its initial user interface.

UIApplicationSceneManifest

The information about the app’s scene-based life-cycle support.

class UISceneConfiguration

Information about the objects and storyboard for UKit to use when creating a particular scene.

class UISceneSession

An object that contains information about one of your app’s scenes.

### Activation and destruction

class UISceneActivationConditions

The set of conditions that define when UIKit activates the current scene.

class ActivationRequestOptions

An object that contains information you want the system to use when activating the session associated with a scene.

class UIWindowSceneDestructionRequestOptions

An object that contains information to use when removing a window scene from your app.

class UISceneDestructionRequestOptions

An object you pass to UIKit to permanently remove a scene and its associated session from your app.

### URL management

class UIOpenURLContext

A system-provided object that contains the information you need to open a single URL.

class OpenExternalURLOptions

Options you specify when asking a scene to open a URL.

### Errors

enum Code

Error codes for issues with scenes.

struct UISceneError

Errors returned during the creation or management of a scene.

let UISceneErrorDomain: String

The domain for scene-related errors.

## See Also

### Life cycle

Managing your app’s life cycle

Respond to system notifications when your app is in the foreground or background, and handle other significant system-related events.

Responding to the launch of your app

Initialize your app’s data structures, prepare your app to run, and respond to any launch-time requests from the system.

class UIApplication

The centralized point of control and coordination for apps running in iOS.

protocol UIApplicationDelegate

A set of methods to manage shared behaviors for your app.

