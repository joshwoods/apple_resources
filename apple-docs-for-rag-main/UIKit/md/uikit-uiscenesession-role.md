

- UIKit
- UISceneSession
-  role 

Instance Property

# role

The role played by the scene’s content.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+tvOS 13.0+visionOS 1.0+

``` source
@MainActor
var role: UISceneSession.Role { get }
```

## Discussion

Use this property to determine how the user interacts with the content of the associated scene. UIKit sets the initial value of this property based on the information in your app’s `Info.plist` file. If you don’t provide scene configuration data for your app, UIKit sets the role to an appropriate value.

## See Also

### Getting the scene information

var scene: UIScene?

The scene associated with the current session.

struct Role

Constants that indicate the possible roles for a scene.

