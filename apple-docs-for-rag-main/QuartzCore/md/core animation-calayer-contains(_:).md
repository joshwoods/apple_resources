

- Core Animation
- CALayer
-  contains(\_:) 

Instance Method

# contains(\_:)

Returns whether the receiver contains a specified point.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+

``` source
func contains(_ p: CGPoint) -> Bool
```

## Parameters 

`p`  

A point in the receiver’s coordinate system.

## Return Value

true if the bounds of the layer contains the point.

## See Also

### Hit Testing

func hitTest(CGPoint) -> CALayer?

Returns the farthest descendant of the receiver in the layer hierarchy (including itself) that contains the specified point.

