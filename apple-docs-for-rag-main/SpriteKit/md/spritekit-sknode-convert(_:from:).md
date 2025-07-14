

- SpriteKit
- SKNode
-  convert(\_:from:) 

Instance Method

# convert(\_:from:)

Converts a point from the coordinate system of another node in the node tree to the coordinate system of this node.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

**watchOS**

``` source
func convert(
    _ point: CGPoint,
    from node: SKNode
) -> CGPoint
```

**iOS, iPadOS, Mac Catalyst, macOS, tvOS, visionOS**

``` source
@MainActor
func convert(
    _ point: CGPoint,
    from node: SKNode
) -> CGPoint
```

## Parameters 

`point`  

A point in the other node’s coordinate system.

`node`  

Another node in the same node tree as this node.

## Return Value

The same point converted to this node’s coordinate system.

## See Also

### Converting Between Coordinate Systems of Different Nodes

Converting Coordinate Spaces

Convert positions across the various coordinate spaces in a scene.

func convert(CGPoint, to: SKNode) -> CGPoint

Converts a point in this node’s coordinate system to the coordinate system of another node in the node tree.

