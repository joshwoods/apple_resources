

- ARKit
- ARSKView
-  session 

Instance Property

# session

The AR session that manages motion tracking and camera image processing for the view’s contents.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+

``` source
@MainActor
var session: ARSession { get set }
```

## Discussion

A view creates its own session object; use this property to access and configure the view’s session.

## See Also

### First Steps

Providing 2D Virtual Content with SpriteKit

Use SpriteKit to place two-dimensional images in 3D space in your AR experience.

