

- Foundation
- NSCoder
-  cgPoint(for:) 

Type Method

# cgPoint(for:)

Returns a Core Graphics point structure corresponding to the data in a given string.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
class func cgPoint(for string: String) -> CGPoint
```

## Parameters 

`string`  

A string whose contents are of the form “{*x*,*y*}”, where *x* is the x coordinate and *y* is the y coordinate. The *x* and *y* values can represent integer or float values. An example of a valid string is @”{3.0,2.5}”. The string is not localized, so items are always separated with a comma.

## Return Value

A Core Graphics structure that represents a point. If the string is not well-formed, the function returns CGPointZero.

## Discussion

In general, you should use this function only to convert strings that were previously created using the string(for:) function.

## See Also

### Representing Geometric Types as Strings

class func cgAffineTransform(for: String) -> CGAffineTransform

Returns a Core Graphics affine transform structure corresponding to the data in a given string.

class func cgRect(for: String) -> CGRect

Returns a Core Graphics rectangle structure corresponding to the data in a given string.

class func cgSize(for: String) -> CGSize

Returns a Core Graphics size structure corresponding to the data in a given string.

class func cgVector(for: String) -> CGVector

Returns a Core Graphics vector corresponding to the data in a given string.

class func nsDirectionalEdgeInsets(for: String) -> NSDirectionalEdgeInsets

Returns a directional edge insets structure based on data in the specified string.

class func uiEdgeInsets(for: String) -> UIEdgeInsets

Returns a UIKit edge insets structure based on the data in the specified string.

class func uiOffset(for: String) -> UIOffset

Returns a UIKit offset structure corresponding to the data in a given string.

class func string(for: CGRect) -> String

Returns a string formatted to contain the data from a rectangle.

class func string(for: CGVector) -> String

Returns a string formatted to contain the data from a vector data structure.

class func string(for: CGAffineTransform) -> String

Returns a string formatted to contain the data from an affine transform.

class func string(for: CGPoint) -> String

Returns a string formatted to contain the data from a point.

class func string(for: CGSize) -> String

Returns a string formatted to contain the data from a size data structure.

class func string(for: NSDirectionalEdgeInsets) -> String

Returns a string formatted to contain the data from a directional edge insets structure.

class func string(for: UIEdgeInsets) -> String

Returns a string formatted to contain the data from an edge insets structure.

class func string(for: UIOffset) -> String

Returns a string formatted to contain the data from an offset structure.

