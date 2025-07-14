

- Foundation
-  NSStringFromSize(\_:) 

Function

# NSStringFromSize(\_:)

Returns a string representation of a size.

Mac Catalyst 13.0+macOS 10.0+

``` source
func NSStringFromSize(_ aSize: NSSize) -> String
```

## Return Value

A string of the form “{a, b}”, where a and b are the width and height, respectively, of `aSize`.

## See Also

### Managing Sizes

func NSEqualSizes(NSSize, NSSize) -> Bool

Returns a Boolean that indicates whether two size values are equal.

func NSMakeSize(Double, Double) -> NSSize

Returns a new `NSSize` from the specified values.

func NSSizeFromString(String) -> NSSize

Returns an `NSSize` from a text-based representation.

func NSSizeFromCGSize(CGSize) -> NSSize

Returns an `NSSize` typecast from a `CGSize`.

func NSSizeToCGSize(NSSize) -> CGSize

Returns a `CGSize` typecast from an `NSSize`.

