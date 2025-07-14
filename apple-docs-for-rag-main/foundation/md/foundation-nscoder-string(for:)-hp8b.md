

- Foundation
- NSCoder
-  string(for:) 

Type Method

# string(for:)

Returns a string formatted to contain the data from a directional edge insets structure.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+tvOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
class func string(for insets: NSDirectionalEdgeInsets) -> String
```

## Parameters 

`insets`  

A directional edge insets data structure.

## Return Value

A string that corresponds to insets. See nsDirectionalEdgeInsets(for:) for a discussion of the string format.

## See Also

### Representing Geometric Types as Strings

class func cgAffineTransform(for: String) -> CGAffineTransform

Returns a Core Graphics affine transform structure corresponding to the data in a given string.

class func cgPoint(for: String) -> CGPoint

Returns a Core Graphics point structure corresponding to the data in a given string.

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

class func string(for: UIEdgeInsets) -> String

Returns a string formatted to contain the data from an edge insets structure.

class func string(for: UIOffset) -> String

Returns a string formatted to contain the data from an offset structure.

