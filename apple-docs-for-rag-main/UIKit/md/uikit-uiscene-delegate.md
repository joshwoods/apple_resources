

- UIKit
- UIScene
-  delegate 

Instance Property

# delegate

The object you use to receive life-cycle events associated with the scene.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+tvOS 13.0+visionOS 1.0+

``` source
@MainActor
var delegate: (any UISceneDelegate)? { get set }
```

## Discussion

The system creates a default delegate object based on the the class name you provide in your app’s `Info.plist` file, or that your app delegate specifies when configuring the scene. You can change this default delegate object later, as needed.

## See Also

### Managing the life cycle of a scene

protocol UISceneDelegate

The core methods you use to respond to life-cycle events occurring within a scene.

