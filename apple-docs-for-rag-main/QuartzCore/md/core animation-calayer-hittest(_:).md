

- Core Animation
- CALayer
-  hitTest(\_:) 

Instance Method

# hitTest(\_:)

Returns the farthest descendant of the receiver in the layer hierarchy (including itself) that contains the specified point.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+

``` source
func hitTest(_ p: CGPoint) -> CALayer?
```

## Parameters 

`p`  

A point in the coordinate system of the receiver’s superlayer.

## Return Value

The layer that contains `thePoint` or `nil` if the point lies outside the receiver’s bounds rectangle.

## See Also

### Hit Testing

func contains(CGPoint) -> Bool

Returns whether the receiver contains a specified point.

