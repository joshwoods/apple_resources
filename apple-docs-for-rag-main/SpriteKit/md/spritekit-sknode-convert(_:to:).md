

- SpriteKit
- SKNode
-  convert(\_:to:) 

Instance Method

# convert(\_:to:)

Converts a point in this node’s coordinate system to the coordinate system of another node in the node tree.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

**iOS, iPadOS, Mac Catalyst, macOS, tvOS, visionOS**

``` source
@MainActor
func convert(
    _ point: CGPoint,
    to node: SKNode
) -> CGPoint
```

**watchOS**

``` source
func convert(
    _ point: CGPoint,
    to node: SKNode
) -> CGPoint
```

## Parameters 

`point`  

A point in this node’s coordinate system.

`node`  

Another node in the same node tree as this node.

## Return Value

The same point converted to the other node’s coordinate system.

## Mentioned in 

Converting Coordinate Spaces

Connecting Bodies with Joints

## See Also

### Converting Between Coordinate Systems of Different Nodes

Converting Coordinate Spaces

Convert positions across the various coordinate spaces in a scene.

func convert(CGPoint, from: SKNode) -> CGPoint

Converts a point from the coordinate system of another node in the node tree to the coordinate system of this node.

