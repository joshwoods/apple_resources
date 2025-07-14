

- SpriteKit
- SKNode
-  yScale 

Instance Property

# yScale

A scaling factor that multiplies the height of a node and its children.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

**watchOS**

``` source
var yScale: CGFloat { get set }
```

**iOS, iPadOS, Mac Catalyst, macOS, tvOS, visionOS**

``` source
@MainActor
var yScale: CGFloat { get set }
```

## Mentioned in 

Resizing a Sprite in Nine Parts

Getting Started with a Camera

Getting Started with Nodes

About Node Property Propagation

## Discussion

The yScale property scales the height of the node and all of its descendants. The scale value affects how a node’s frame is calculated, its hit test area, how it is drawn, and other similar characteristics. The default value is `1.0`.

## See Also

### Scaling and Rotating

var zRotation: CGFloat

The Euler rotation about the z axis (in radians).

func setScale(CGFloat)

Sets the xScale and yScale properties of the node.

var xScale: CGFloat

A scaling factor that multiplies the width of a node and its children.

