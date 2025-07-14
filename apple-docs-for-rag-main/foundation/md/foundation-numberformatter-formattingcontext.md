

- Foundation
- NumberFormatter
-  formattingContext 

Instance Property

# formattingContext

The capitalization formatting context used when formatting a number.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var formattingContext: Formatter.Context { get set }
```

## Discussion

Defaults to NSFormattingContextUnknown.

## See Also

### Configuring Numeric Formats

var format: String

The receiver’s format.

var formatWidth: Int

The format width used by the receiver.

var negativeFormat: String!

The format the receiver uses to display negative values.

var positiveFormat: String!

The format the receiver uses to display positive values.

var multiplier: NSNumber?

The multiplier of the receiver.

