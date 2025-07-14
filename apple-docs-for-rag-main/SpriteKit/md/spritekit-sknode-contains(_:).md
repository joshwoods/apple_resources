

- SpriteKit
- SKNode
-  contains(\_:) 

Instance Method

# contains(\_:)

Returns a Boolean value that indicates whether a point lies inside the parent’s coordinate system.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

**watchOS**

``` source
func contains(_ p: CGPoint) -> Bool
```

**iOS, iPadOS, Mac Catalyst, macOS, tvOS, visionOS**

``` source
@MainActor
func contains(_ p: CGPoint) -> Bool
```

## Parameters 

`p`  

A `CGPoint` to test against.

## Return Value

true if the point lies inside the parent’s coordinate system; otherwise false.

## See Also

### Hit Testing

Understanding Hit-Testing

Learn how find child nodes at a given point by using hit-testing.

func atPoint(CGPoint) -> SKNode

Returns the deepest visible descendant that intersects a point.

func nodes(at: CGPoint) -> [SKNode]

Returns an array of all visible descendants that intersect a point.

