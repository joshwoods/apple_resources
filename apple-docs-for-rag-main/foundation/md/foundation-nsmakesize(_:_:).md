

- Foundation
-  NSMakeSize(\_:\_:) 

Function

# NSMakeSize(\_:\_:)

Returns a new `NSSize` from the specified values.

Mac Catalyst 13.0+macOS 10.0+

``` source
func NSMakeSize(
    _ w: Double,
    _ h: Double
) -> NSSize
```

## Return Value

An `NSSize` having the specified `width` and `height`.

## See Also

### Managing Sizes

func NSEqualSizes(NSSize, NSSize) -> Bool

Returns a Boolean that indicates whether two size values are equal.

func NSSizeFromString(String) -> NSSize

Returns an `NSSize` from a text-based representation.

func NSStringFromSize(NSSize) -> String

Returns a string representation of a size.

func NSSizeFromCGSize(CGSize) -> NSSize

Returns an `NSSize` typecast from a `CGSize`.

func NSSizeToCGSize(NSSize) -> CGSize

Returns a `CGSize` typecast from an `NSSize`.

