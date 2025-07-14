

- UIKit
- UIWindowScene
- UIWindowScene.GeometryPreferences
- UIWindowScene.GeometryPreferences.iOS
-  interfaceOrientations 

Instance Property

# interfaceOrientations

The preferred interface orientations for the scene.

iOS 16.0+iPadOS 16.0+Mac CatalystvisionOS

``` source
var interfaceOrientations: UIInterfaceOrientationMask? { get set }
```

## Discussion

If you specify this value, the system automatically chooses an orientation from the intersection of these preferred orientations and the supported orientations.

