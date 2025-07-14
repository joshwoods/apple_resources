

- Foundation
- NumberFormatter
-  attributedStringForZero 

Instance Property

# attributedStringForZero

The attributed string that the receiver uses to display zero values.

macOS 10.0+

``` source
@NSCopying
var attributedStringForZero: NSAttributedString { get set }
```

## Discussion

By default zero values are displayed according to the format specified for positive values; for more discussion of this subject see Data Formatting Guide.

### Special Considerations

This method is for use with formatters using `NSNumberFormatterBehavior10_0` behavior.

## See Also

### Configuring the Display of Numeric Values

var textAttributesForNegativeValues: [String : Any]?

The text attributes to be used in displaying negative values.

var textAttributesForPositiveValues: [String : Any]?

The text attributes to be used in displaying positive values.

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

