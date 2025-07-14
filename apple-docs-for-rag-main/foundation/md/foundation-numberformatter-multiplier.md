

- Foundation
- NumberFormatter
-  multiplier 

Instance Property

# multiplier

The multiplier of the receiver.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
@NSCopying
var multiplier: NSNumber? { get set }
```

## Discussion

A multiplier is a factor used in conversions between numbers and strings (that is, numbers as stored and numbers as displayed). When the input value is a string, the multiplier is used to divide, and when the input value is a number, the multiplier is used to multiply. These operations allow the formatted values to be different from the values that a program manipulates internally.

## See Also

### Configuring Numeric Formats

var format: String

The receiver’s format.

var formattingContext: Formatter.Context

The capitalization formatting context used when formatting a number.

var formatWidth: Int

The format width used by the receiver.

var negativeFormat: String!

The format the receiver uses to display negative values.

var positiveFormat: String!

The format the receiver uses to display positive values.

