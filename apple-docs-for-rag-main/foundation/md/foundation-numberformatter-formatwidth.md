

- Foundation
- NumberFormatter
-  formatWidth 

Instance Property

# formatWidth

The format width used by the receiver.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var formatWidth: Int { get set }
```

## Discussion

The format width is the number of characters of a formatted number within a string that is either left justified or right justified based on the value contained in paddingPosition.

## See Also

### Configuring Numeric Formats

var format: String

The receiver’s format.

var formattingContext: Formatter.Context

The capitalization formatting context used when formatting a number.

var negativeFormat: String!

The format the receiver uses to display negative values.

var positiveFormat: String!

The format the receiver uses to display positive values.

var multiplier: NSNumber?

The multiplier of the receiver.

