

- SpriteKit
- SKNode
-  frame 

Instance Property

# frame

A rectangle in the parent’s coordinate system that contains the node’s content, ignoring the node’s children.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

**iOS, iPadOS, Mac Catalyst, macOS, tvOS, visionOS**

``` source
@MainActor
var frame: CGRect { get }
```

**watchOS**

``` source
var frame: CGRect { get }
```

## Mentioned in 

Getting Started with Nodes

Resizing a Sprite in Nine Parts

Getting Started with Sprite Nodes

Positioning a Scene’s Origin Within its View

## Discussion

The frame is the smallest rectangle that contains the node’s content, taking into account the node’s xScale, yScale, and zRotation properties.

Since `SKNode` does not draw content of its own, its frame size is arbitrary; it’s the visual subclasses of `SKNode` that do draw that define the frame’s size with a meaningful value that encloses its visual content.

To get a rect that encloses all the child nodes of an `SKNode` parent object, use calculateAccumulatedFrame().

## See Also

### Querying the Content Size

func calculateAccumulatedFrame() -> CGRect

Returns a rectangle in the parent’s coordinate system that contains the position and size of itself and all child nodes.

