

- UIKit
- UIScene
-  session 

Instance Property

# session

The session associated with the scene.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+tvOS 13.0+visionOS 1.0+

``` source
@MainActor
var session: UISceneSession { get }
```

## Discussion

UIKit maintains a session object for each scene. The session object contains a unique identifier for the scene and other information about its configuration.

## See Also

### Getting the scene’s session

class UISceneSession

An object that contains information about one of your app’s scenes.

