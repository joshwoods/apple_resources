

- UIKit
- UISceneConfiguration
-  role 

Instance Property

# role

The role assigned to the scene configuration.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+tvOS 13.0+visionOS 1.0+

``` source
@MainActor
var role: UISceneSession.Role { get }
```

## Discussion

UIKit populates this property with an appropriate role value based on the contents of your app’s `Info.plist` file. You also specify this value when you create a new scene-configuration object.

## See Also

### Getting the configuration attributes

var name: String?

The app-specific name assigned to the scene configuration.

struct Role

Constants that indicate the possible roles for a scene.

