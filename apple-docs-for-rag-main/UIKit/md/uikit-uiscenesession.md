

- UIKit
-  UISceneSession 

Class

# UISceneSession

An object that contains information about one of your app’s scenes.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+tvOS 13.0+visionOS 1.0+

``` source
@MainActor
class UISceneSession
```

## Overview

A UISceneSession object manages a unique runtime instance of your scene. When the user adds a new scene to your app, or when you request one programmatically, the system creates a session object to track that scene. The session contains a unique identifier and the configuration details of the scene. UIKit maintains the session information for the lifetime of the scene itself, destroying the session in response to the user closing the scene in the app switcher.

You don’t create session objects directly. UIKit creates sessions in response to user interactions with your app. You can also ask UIKit to create a new scene and session programmatically by calling the requestSceneSessionActivation(_:userActivity:options:errorHandler:) method of UIApplication. UIKit initializes the session with default configuration data based on the contents of your app’s `Info.plist` file.

## Topics

### Getting the scene information

var scene: UIScene?

The scene associated with the current session.

var role: UISceneSession.Role

The role played by the scene’s content.

struct Role

Constants that indicate the possible roles for a scene.

### Getting the scene configuration details

var configuration: UISceneConfiguration

The configuration data for creating the scene.

class UISceneConfiguration

Information about the objects and storyboard for UKit to use when creating a particular scene.

### Identifying the scene

var persistentIdentifier: String

A unique identifier that persists for the lifetime of the session.

### Getting additional session information

var stateRestorationActivity: NSUserActivity?

An activity object you can use to restore the previous contents of your scene’s interface.

var userInfo: [String : Any]?

Custom attributes that you can associate with the scene.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSObjectProtocol
- NSSecureCoding
- Sendable

## See Also

### Configuration

Specifying the scenes your app supports

Tell the system about your app’s scenes, including the objects you use to manage each scene and its initial user interface.

UIApplicationSceneManifest

The information about the app’s scene-based life-cycle support.

class UISceneConfiguration

Information about the objects and storyboard for UKit to use when creating a particular scene.

