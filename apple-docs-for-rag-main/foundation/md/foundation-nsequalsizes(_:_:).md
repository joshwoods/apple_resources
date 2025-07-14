

- Foundation
-  NSEqualSizes(\_:\_:) 

Function

# NSEqualSizes(\_:\_:)

Returns a Boolean that indicates whether two size values are equal.

Mac Catalyst 13.0+macOS 10.0+

``` source
func NSEqualSizes(
    _ aSize: NSSize,
    _ bSize: NSSize
) -> Bool
```

## Return Value

true if `aSize` and `bSize` are identical, otherwise false.

## See Also

### Managing Sizes

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

