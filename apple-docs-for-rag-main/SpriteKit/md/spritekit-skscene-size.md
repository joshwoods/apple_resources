

- SpriteKit
- SKScene
-  size 

Instance Property

# size

The dimensions of the scene, in points.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

**iOS, iPadOS, Mac Catalyst, macOS, tvOS, visionOS**

``` source
@MainActor
var size: CGSize { get set }
```

**watchOS**

``` source
var size: CGSize { get set }
```

## Discussion

When a scene is first initialized, its size property is configured by the designated initializer. The size of the scene specifies the size of the visible portion of the scene in points. This is only used to specify the visible portion of the scene. Nodes in the tree can be positioned outside of this area; those nodes are still processed by the scene, but are ignored by the renderer.

When a scene is presented, the size and anchorPoint properties determine the portion of the scene’s coordinate space that is visible in the view.

If you set the size property to a new value, the scene’s didChangeSize(_:) method is called. This property can also change if the scaleMode property is set to SKSceneScaleMode.resizeFill and the presenting view is resized. After the scene’s size changes, future updates are rendered immediately at the new size.

## See Also

### Creating a Scene Programmatically

init(size: CGSize)

Initializes a new scene object.

