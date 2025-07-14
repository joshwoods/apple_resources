

- SpriteKit
- SKVideoNode
-  anchorPoint 

Instance Property

# anchorPoint

The point in the sprite that corresponds to the node’s position.

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

Adding a Video to a Scene

## Discussion

You specify the anchor point using the unit coordinate space. The default value is `(0.5,0.5)`, which means that the video is centered on the node’s position.

## See Also

### Setting the Video Node’s Visual Properties

var size: CGSize

The dimensions of the video node, in points.

