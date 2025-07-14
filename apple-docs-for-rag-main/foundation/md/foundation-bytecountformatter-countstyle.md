

- Foundation
- ByteCountFormatter
-  countStyle 

Instance Property

# countStyle

Specify the number of bytes to be used for kilobytes.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+macOS 10.8+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var countStyle: ByteCountFormatter.CountStyle { get set }
```

## Discussion

The default setting is ByteCountFormatter.CountStyle.file, which is the system specific value for file and storage sizes.

## See Also

### Setting Formatting Styles

var formattingContext: Formatter.Context

Specify the formatting context for the formatted string.

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

