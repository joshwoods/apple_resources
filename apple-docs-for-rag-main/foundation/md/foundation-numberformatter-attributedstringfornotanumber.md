

- Foundation
- NumberFormatter
-  attributedStringForNotANumber 

Instance Property

# attributedStringForNotANumber

The attributed string the receiver uses to display “not a number” values.

macOS 10.0+

``` source
@NSCopying
var attributedStringForNotANumber: NSAttributedString { get set }
```

## Discussion

By default “not a number” values are displayed as the string “NaN”.

### Special Considerations

This method is for use with formatters using `NSNumberFormatterBehavior10_0` behavior.

## See Also

### Configuring the Display of Numeric Values

var textAttributesForNegativeValues: [String : Any]?

The text attributes to be used in displaying negative values.

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

var textAttributesForNotANumber: [String : Any]?

The text attributes used to display the NaN (“not a number”) string.

var textAttributesForPositiveInfinity: [String : Any]?

The text attributes used to display the positive infinity symbol.

var textAttributesForNegativeInfinity: [String : Any]?

The text attributes used to display the negative infinity symbol.

