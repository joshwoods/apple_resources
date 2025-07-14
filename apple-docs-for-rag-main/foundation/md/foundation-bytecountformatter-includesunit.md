

- Foundation
- ByteCountFormatter
-  includesUnit 

Instance Property

# includesUnit

Determines whether to include the units in the resulting formatted string.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+macOS 10.8+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var includesUnit: Bool { get set }
```

## Discussion

If set to true and includesCount is set to false, no count is displayed. For example, a value of 723 KB is formatted as `KB`.

You can get the set this property to true and the includesCount to true individually to get both parts, separately. Note that putting them together yourself via string concatenation may be incorrect for some locales.

The default value is true.

Note

Setting this value to false and includesCount to false results in an empty string.

## See Also

### Setting Formatting Styles

var formattingContext: Formatter.Context

Specify the formatting context for the formatted string.

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

var zeroPadsFractionDigits: Bool

Determines whether to zero pad fraction digits so a consistent number of characters is displayed in a representation.

