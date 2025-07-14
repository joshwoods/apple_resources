

- SpriteKit
- SKScene
-  anchorPoint 

Instance Property

# anchorPoint

The point in the view’s frame that corresponds to the scene’s origin.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

**watchOS**

``` source
var anchorPoint: CGPoint { get set }
```

**iOS, iPadOS, Mac Catalyst, macOS, tvOS, visionOS**

``` source
@MainActor
var anchorPoint: CGPoint { get set }
```

## Mentioned in 

Positioning a Scene’s Origin Within its View

Drawing SpriteKit Content in a View

Getting Started with a Camera

## Discussion

When a scene is presented and a camera node has not been specified, the size and anchorPoint properties determine which part of the scene’s coordinate space is visible in the view.

You specify the value using the unit coordinate space. The default value is `(0,0)`, which corresponds to the lower-left corner of the view’s frame rectangle.

## See Also

### Configuring the Viewport

Positioning a Scene’s Origin Within its View

Try the different ways to configure the scene’s origin inside its view.

var camera: SKCameraNode?

The camera node in the scene that determines what part of the scene’s coordinate space is visible in the view.

