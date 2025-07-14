

- Foundation
- NumberFormatter
-  textAttributesForNegativeValues 

Instance Property

# textAttributesForNegativeValues

The text attributes to be used in displaying negative values.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var textAttributesForNegativeValues: [String : Any]? { get set }
```

## Discussion

This property is a dictionary that contains the attributes used to display negative values.

## See Also

### Configuring the Display of Numeric Values

var textAttributesForPositiveValues: [String : Any]?

The text attributes to be used in displaying positive values.

var attributedStringForZero: NSAttributedString

The attributed string that the receiver uses to display zero values.

var textAttributesForZero: [String : Any]?

The text attributes used to display a zero value.

var attributedStringForNil: NSAttributedString

The attributed string the receiver uses to display `nil` values.

var textAttributesForNil: [String : Any]?

The text attributes used to display the `nil` symbol.

var attributedStringForNotANumber: NSAttributedString

The attributed string the receiver uses to display “not a number” values.

var textAttributesForNotANumber: [String : Any]?

The text attributes used to display the NaN (“not a number”) string.

var textAttributesForPositiveInfinity: [String : Any]?

The text attributes used to display the positive infinity symbol.

var textAttributesForNegativeInfinity: [String : Any]?

The text attributes used to display the negative infinity symbol.

