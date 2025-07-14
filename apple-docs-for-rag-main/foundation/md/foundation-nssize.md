

- Foundation
-  NSSize 

Type Alias

# NSSize

A two-dimensional size.

Mac Catalyst 13.0+macOS 10.0+

``` source
typealias NSSize = CGSize
```

## Discussion

Normally, the values of `width` and `height` are non-negative. The functions that create an `NSSize` structure do not prevent you from setting a negative value for these attributes. If the value of `width` or `height` is negative, however, the behavior of some methods may be undefined.

### Special Considerations

Prior to OS X v10.5 the width and height were represented by `float` values rather than `CGFloat` values.

When building for 64 bit systems, or building 32 bit like 64 bit, `NSSize` is typedef’d to `CGSize`.

## Topics

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

func NSSizeToCGSize(NSSize) -> CGSize

Returns a `CGSize` typecast from an `NSSize`.

### Zero Constant

let NSZeroSize: NSSize

An `NSSize` structure set to `0` in both dimensions.

### Related Types

typealias NSSizeArray

Type indicating a parameter is an array of `NSSize` structures.

typealias NSSizePointer

Type indicating parameter is a pointer to an `NSSize` structure.

## See Also

### Geometry

@frozen struct CGFloat

The basic type for floating-point scalar values in Core Graphics and related frameworks.

typealias NSPoint

A point in a Cartesian coordinate system.

typealias NSRect

A rectangle.

struct AffineTransform

A graphics coordinate transformation.

struct NSEdgeInsets

A description of the distance between the edges of two rectangles.

