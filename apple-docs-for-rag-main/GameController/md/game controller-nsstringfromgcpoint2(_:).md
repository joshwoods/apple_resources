

- Game Controller
-  NSStringFromGCPoint2(\_:) 

Function

# NSStringFromGCPoint2(\_:)

Returns a string representation of a point.

iOS 17.4+iPadOS 17.4+Mac Catalyst 17.4+macOS 14.3+tvOS 17.4+visionOS 1.1+

``` source
func NSStringFromGCPoint2(_ point: GCPoint2) -> String
```

## Parameters 

`point`  

The point to convert to a string.

## Return Value

A string of the form `{a, b}`, where `a` and `b` are the x and y coordinates of `point`.

## See Also

### Comparing and converting points

func GCPoint2Equal(GCPoint2, GCPoint2) -> Bool

Returns whether two points are equal.

