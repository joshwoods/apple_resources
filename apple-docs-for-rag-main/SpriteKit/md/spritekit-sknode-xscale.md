

- SpriteKit
- SKNode
-  xScale 

Instance Property

# xScale

A scaling factor that multiplies the width of a node and its children.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

**iOS, iPadOS, Mac Catalyst, macOS, tvOS, visionOS**

``` source
@MainActor
var xScale: CGFloat { get set }
```

**watchOS**

``` source
var xScale: CGFloat { get set }
```

## Mentioned in 

Resizing a Sprite in Nine Parts

Getting Started with a Camera

About Node Property Propagation

Getting Started with Nodes

## Discussion

The xScale property scales the width of the node and all of its descendants. The scale value affects how a node’s frame is calculated, its hit test area, how it is drawn, and other similar characteristics. The default value is `1.0`.

## See Also

### Scaling and Rotating

var zRotation: CGFloat

The Euler rotation about the z axis (in radians).

func setScale(CGFloat)

Sets the xScale and yScale properties of the node.

var yScale: CGFloat

A scaling factor that multiplies the height of a node and its children.

