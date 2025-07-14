

- Foundation
-  NSPointFromString(\_:) 

Function

# NSPointFromString(\_:)

Returns a point from a text-based representation.

Mac Catalyst 13.0+macOS 10.0+

``` source
func NSPointFromString(_ aString: String) -> NSPoint
```

## Parameters 

`aString`  

A string of the form “{x, y}”.

## Return Value

If `aString` is of the form “{x, y}” an `NSPoint` structure that uses x and y as the x and y coordinates, in that order.

## Discussion

If `aString` only contains a single number, it is used as the x coordinate. If `aString` does not contain any numbers, returns an `NSPoint` object whose x and y coordinates are both 0.

## See Also

### Managing Points

func NSEqualPoints(NSPoint, NSPoint) -> Bool

Returns a Boolean value that indicates whether two points are equal.

func NSMakePoint(Double, Double) -> NSPoint

Creates a new `NSPoint` from the specified values.

func NSStringFromPoint(NSPoint) -> String

Returns a string representation of a point.

func NSPointFromCGPoint(CGPoint) -> NSPoint

Returns an `NSPoint` typecast from a `CGPoint`.

func NSPointToCGPoint(NSPoint) -> CGPoint

Returns a `CGPoint` typecast from an `NSPoint`.

