

- SpriteKit
- SKNode
-  calculateAccumulatedFrame() 

Instance Method

# calculateAccumulatedFrame()

Returns a rectangle in the parent’s coordinate system that contains the position and size of itself and all child nodes.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

**iOS, iPadOS, Mac Catalyst, macOS, tvOS, visionOS**

``` source
@MainActor
func calculateAccumulatedFrame() -> CGRect
```

**watchOS**

``` source
func calculateAccumulatedFrame() -> CGRect
```

## Mentioned in 

Getting Started with Nodes

Controlling User Interaction on Nodes

## Discussion

The frame takes into the account the cumulative effect of the xScale, yScale, and zRotation properties of each node in the subtree.

Listing 1 shows, in Swift, how calculateAccumulatedFrame() can be used display the bounding box of a shape node. The child node, although smaller than its parent, is rotated by 30° so that its bounds extend beyond its parent’s bounds. After `childNode` has been added to `parentNode`, a further shape node, `boundingBoxNode`, is created with its size based on the accumulated frame of parentNode.

Listing 1. Displaying the accumulated frame of a shape node

```
let parentNode = SKShapeNode(rectOf: CGSize(width: 500, height: 500))
parentNode.lineWidth = 2
parentNode.strokeColor = .blue
parentNode.fillColor = .clear

let childNode = SKShapeNode(rectOf: CGSize(width: 400, height: 400))
childNode.strokeColor = .red
childNode.fillColor = .clear
childNode.zRotation = -CGFloat.pi / 6 // pi / 6 = 30°

parentNode.addChild(childNode)

let boundingBoxNode = SKShapeNode(rectOf: parentNode.calculateAccumulatedFrame().size)
boundingBoxNode.lineWidth = 1
boundingBoxNode.strokeColor = .black
boundingBoxNode.fillColor = .clear
boundingBoxNode.path = boundingBoxNode.path?.copy(dashingWithPhase: 0,
                                                  lengths: [10,10])

parentNode.addChild(boundingBoxNode)
```

The figure below shows the result of Listing 1 with `parentNode` rendered in blue, `childNode` rendered in red and the `boundingBoxNode` rendered with a dashed line.

## See Also

### Querying the Content Size

var frame: CGRect

A rectangle in the parent’s coordinate system that contains the node’s content, ignoring the node’s children.

