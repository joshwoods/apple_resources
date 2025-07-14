

- Foundation
- ByteCountFormatter
-  allowsNonnumericFormatting 

Instance Property

# allowsNonnumericFormatting

Determines whether to allow more natural display of some values.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+macOS 10.8+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var allowsNonnumericFormatting: Bool { get set }
```

## Discussion

Displays a more natural display of some values, such as zero, where it may be displayed as `Zero KB`, ignoring all other flags or options (with the exception of useBytes, which would generate `Zero bytes`).The result is appropriate for standalone output.

Special handling of certain values such as zero is especially important in some languages, so it’s highly recommended that this property be left in its default state.

Default value is true.

## See Also

### Setting Formatting Styles

var formattingContext: Formatter.Context

Specify the formatting context for the formatted string.

var countStyle: ByteCountFormatter.CountStyle

Specify the number of bytes to be used for kilobytes.

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

