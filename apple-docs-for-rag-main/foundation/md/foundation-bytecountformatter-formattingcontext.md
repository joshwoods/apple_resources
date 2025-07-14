

- Foundation
- ByteCountFormatter
-  formattingContext 

Instance Property

# formattingContext

Specify the formatting context for the formatted string.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var formattingContext: Formatter.Context { get set }
```

## Discussion

The default value is `NSFormattingContextUnknown`. See Formatter for possible values.

## See Also

### Setting Formatting Styles

var countStyle: ByteCountFormatter.CountStyle

Specify the number of bytes to be used for kilobytes.

var allowsNonnumericFormatting: Bool

Determines whether to allow more natural display of some values.

var includesActualByteCount: Bool

Determines whether to include the number of bytes after the formatted string.

var isAdaptive: Bool

Determines the display style of the size representation.

var allowedUnits: ByteCountFormatter.Units

Specify the units that can be used in the output.

var includesCount: Bool

Determines whether to include the count in the resulting formatted string.

var includesUnit: Bool

Determines whether to include the units in the resulting formatted string.

var zeroPadsFractionDigits: Bool

Determines whether to zero pad fraction digits so a consistent number of characters is displayed in a representation.

