

- UIKit
-  UISceneConfiguration 

Class

# UISceneConfiguration

Information about the objects and storyboard for UKit to use when creating a particular scene.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+tvOS 13.0+visionOS 1.0+

``` source
@MainActor
class UISceneConfiguration
```

## Overview

Use a UISceneConfiguration object to specify information that UIKit can use to create a new scene for your app. Specifically, you must provide the class of the specific scene you want, the class of the scene delegate object your app uses to manage scenes of that type, and a storyboard containing the scene’s initial view controller.

When the user requests a new instance of your app’s user interface, UIKit looks in your app’s `Info.plist` file for the configuration data it needs to create the corresponding scene object. It then packages that information into a UISceneConfiguration object and delivers it as part of the session it passes to the application(_:configurationForConnecting:options:) method of your app delegate. You can accept that configuration data as is or create a return a new UISceneConfiguration object with a different set of configuration details.

## Topics

### Creating a configuration object

init(name: String?, sessionRole: UISceneSession.Role)

Creates a scene-configuration object with the specified role and app-specific name.

### Specifying the scene creation details

var sceneClass: AnyClass?

The class of the scene object that you want UIKit to create.

var delegateClass: AnyClass?

The class of the custom delegate object that you want UIKit to create.

var storyboard: UIStoryboard?

The storyboard object that contains your scene’s initial view controller.

### Getting the configuration attributes

var name: String?

The app-specific name assigned to the scene configuration.

var role: UISceneSession.Role

The role assigned to the scene configuration.

struct Role

Constants that indicate the possible roles for a scene.

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
- NSCopying
- NSObjectProtocol
- NSSecureCoding
- Sendable

## See Also

### Configuration

Specifying the scenes your app supports

Tell the system about your app’s scenes, including the objects you use to manage each scene and its initial user interface.

UIApplicationSceneManifest

The information about the app’s scene-based life-cycle support.

class UISceneSession

An object that contains information about one of your app’s scenes.

