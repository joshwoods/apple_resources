

- Foundation
-  NSSizeFromCGSize(\_:) 

Function

# NSSizeFromCGSize(\_:)

Returns an `NSSize` typecast from a `CGSize`.

Mac Catalyst 13.0+macOS 10.0+

``` source
func NSSizeFromCGSize(_ cgsize: CGSize) -> NSSize
```

## Return Value

An `NSSize` typecast from a `CGSize`.

## See Also

### Related Documentation

func NSRectFromCGRect(CGRect) -> NSRect

Returns an `NSRect` typecast from a `CGRect`.

func NSPointFromCGPoint(CGPoint) -> NSPoint

Returns an `NSPoint` typecast from a `CGPoint`.

### Managing Sizes

func NSEqualSizes(NSSize, NSSize) -> Bool

Returns a Boolean that indicates whether two size values are equal.

func NSMakeSize(Double, Double) -> NSSize

Returns a new `NSSize` from the specified values.

func NSSizeFromString(String) -> NSSize

Returns an `NSSize` from a text-based representation.

func NSStringFromSize(NSSize) -> String

Returns a string representation of a size.

func NSSizeToCGSize(NSSize) -> CGSize

Returns a `CGSize` typecast from an `NSSize`.

