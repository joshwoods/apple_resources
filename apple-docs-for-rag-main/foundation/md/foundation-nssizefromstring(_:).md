

- Foundation
-  NSSizeFromString(\_:) 

Function

# NSSizeFromString(\_:)

Returns an `NSSize` from a text-based representation.

Mac Catalyst 13.0+macOS 10.0+

``` source
func NSSizeFromString(_ aString: String) -> NSSize
```

## Discussion

Scans `aString` for two numbers which are used as the width and height, in that order, to create an `NSSize` struct. If `aString` only contains a single number, it is used as the width. The `aString` argument should be formatted like the output of NSStringFromSize(_:), for example, `@"{10,20}"`. If `aString` does not contain any numbers, this function returns an `NSSize` struct whose width and height are both `0`.

## See Also

### Managing Sizes

func NSEqualSizes(NSSize, NSSize) -> Bool

Returns a Boolean that indicates whether two size values are equal.

func NSMakeSize(Double, Double) -> NSSize

Returns a new `NSSize` from the specified values.

func NSStringFromSize(NSSize) -> String

Returns a string representation of a size.

func NSSizeFromCGSize(CGSize) -> NSSize

Returns an `NSSize` typecast from a `CGSize`.

func NSSizeToCGSize(NSSize) -> CGSize

Returns a `CGSize` typecast from an `NSSize`.

