

- SwiftUI
- WorldScalingBehavior
-  dynamic 

Type Property

# dynamic

The window will scale up as it moves further away, maintaining the same angular size.

visionOS 2.0+

``` source
static var dynamic: WorldScalingBehavior { get }
```

## Discussion

Prefer dynamic window scaling for windows that display dense UI or a lot of text. Using dynamic scaling ensures that controls and text remain at a comfortable size regardless of the window’s position.

For further information, see Spatial layout in the Human Interface Guidelines.

