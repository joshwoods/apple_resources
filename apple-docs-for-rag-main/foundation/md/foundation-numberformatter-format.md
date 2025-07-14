

- Foundation
- NumberFormatter
-  format 

Instance Property

# format

The receiver’s format.

macOS 10.0+

``` source
var format: String { get set }
```

## Discussion

The format string uses the format patterns from Unicode Technical Standard #35. For more information, see Data Formatting Guide.

## See Also

### Configuring Numeric Formats

var formattingContext: Formatter.Context

The capitalization formatting context used when formatting a number.

var formatWidth: Int

The format width used by the receiver.

var negativeFormat: String!

The format the receiver uses to display negative values.

var positiveFormat: String!

The format the receiver uses to display positive values.

var multiplier: NSNumber?

The multiplier of the receiver.

