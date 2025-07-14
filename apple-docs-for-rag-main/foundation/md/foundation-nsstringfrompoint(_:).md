

- Foundation
-  NSStringFromPoint(\_:) 

Function

# NSStringFromPoint(\_:)

Returns a string representation of a point.

Mac Catalyst 13.0+macOS 10.0+

``` source
func NSStringFromPoint(_ aPoint: NSPoint) -> String
```

## Parameters 

`aPoint`  

A point structure.

## Return Value

A string of the form “{a, b}”, where a and b are the x and y coordinates of `aPoint`.

## See Also

### Managing Points

func NSEqualPoints(NSPoint, NSPoint) -> Bool

Returns a Boolean value that indicates whether two points are equal.

func NSMakePoint(Double, Double) -> NSPoint

Creates a new `NSPoint` from the specified values.

func NSPointFromString(String) -> NSPoint

Returns a point from a text-based representation.

func NSPointFromCGPoint(CGPoint) -> NSPoint

Returns an `NSPoint` typecast from a `CGPoint`.

func NSPointToCGPoint(NSPoint) -> CGPoint

Returns a `CGPoint` typecast from an `NSPoint`.

