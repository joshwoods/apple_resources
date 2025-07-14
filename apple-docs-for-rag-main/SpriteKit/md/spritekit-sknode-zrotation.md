

- SpriteKit
- SKNode
-  zRotation 

Instance Property

# zRotation

The Euler rotation about the z axis (in radians).

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

**iOS, iPadOS, Mac Catalyst, macOS, tvOS, visionOS**

``` source
@MainActor
var zRotation: CGFloat { get set }
```

**watchOS**

``` source
var zRotation: CGFloat { get set }
```

## Mentioned in 

Getting Started with Nodes

About Node Property Propagation

Making Physics Bodies Move

About SpriteKit Coordinate Systems

Getting Started with a Camera

## Discussion

The default value is `0.0`, which indicates no rotation. A positive value indicates a counterclockwise rotation. When the coordinate system is rotated, it affects the node and its descendants. The rotation affects the node’s frame property, hit testing, rendering, and other similar characteristics.

## See Also

### Scaling and Rotating

func setScale(CGFloat)

Sets the xScale and yScale properties of the node.

var xScale: CGFloat

A scaling factor that multiplies the width of a node and its children.

var yScale: CGFloat

A scaling factor that multiplies the height of a node and its children.

