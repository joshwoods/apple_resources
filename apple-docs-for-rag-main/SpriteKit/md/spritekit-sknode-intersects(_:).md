

- SpriteKit
- SKNode
-  intersects(\_:) 

Instance Method

# intersects(\_:)

Returns a Boolean value that indicates whether this node intersects the specified node.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

**iOS, iPadOS, Mac Catalyst, macOS, tvOS, visionOS**

``` source
@MainActor
func intersects(_ node: SKNode) -> Bool
```

**watchOS**

``` source
func intersects(_ node: SKNode) -> Bool
```

## Parameters 

`node`  

Another node in the same node tree.

## Return Value

true if the two nodes intersect; otherwise false.

## Discussion

The two nodes are considered to intersect if their frames intersect. The children of both nodes are ignored in this test.

