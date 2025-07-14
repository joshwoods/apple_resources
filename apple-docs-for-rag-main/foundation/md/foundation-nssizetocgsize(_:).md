

- Foundation
-  NSSizeToCGSize(\_:) 

Function

# NSSizeToCGSize(\_:)

Returns a `CGSize` typecast from an `NSSize`.

Mac Catalyst 13.0+macOS 10.0+

``` source
func NSSizeToCGSize(_ nssize: NSSize) -> CGSize
```

## Return Value

A `CGSize` typecast from an `NSSize`.

## See Also

### Related Documentation

func NSPointToCGPoint(NSPoint) -> CGPoint

Returns a `CGPoint` typecast from an `NSPoint`.

func NSRectToCGRect(NSRect) -> CGRect

Returns a `CGRect` typecast from an `NSRect`.

### Managing Sizes

func NSEqualSizes(NSSize, NSSize) -> Bool

Returns a Boolean that indicates whether two size values are equal.

func NSMakeSize(Double, Double) -> NSSize

Returns a new `NSSize` from the specified values.

func NSSizeFromString(String) -> NSSize

Returns an `NSSize` from a text-based representation.

func NSStringFromSize(NSSize) -> String

Returns a string representation of a size.

func NSSizeFromCGSize(CGSize) -> NSSize

Returns an `NSSize` typecast from a `CGSize`.

