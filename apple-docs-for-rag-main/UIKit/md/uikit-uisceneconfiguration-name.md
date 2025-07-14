

- UIKit
- UISceneConfiguration
-  name 

Instance Property

# name

The app-specific name assigned to the scene configuration.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+tvOS 13.0+visionOS 1.0+

``` source
@MainActor
var name: String? { get }
```

## Discussion

UIKit sets this property’s initial value using the UISceneConfigurationName key from the appropriate scene in your app’s `Info.plist` file. You also specify this value when you create a new scene-configuration object.

## See Also

### Getting the configuration attributes

var role: UISceneSession.Role

The role assigned to the scene configuration.

struct Role

Constants that indicate the possible roles for a scene.

