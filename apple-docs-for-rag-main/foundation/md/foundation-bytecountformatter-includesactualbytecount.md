

- Foundation
- ByteCountFormatter
-  includesActualByteCount 

Instance Property

# includesActualByteCount

Determines whether to include the number of bytes after the formatted string.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+macOS 10.8+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var includesActualByteCount: Bool { get set }
```

## Discussion

Setting this value to true causes the byte count to be displayed parenthetically (localized as appropriate), for instance `723 KB (722,842 bytes)`. This will happen only if needed, that is, the first part is already not showing the exact byte count.

If includesUnit or includesCount are false, then this setting has no effect.

Default value is false.

## See Also

### Setting Formatting Styles

var formattingContext: Formatter.Context

Specify the formatting context for the formatted string.

var countStyle: ByteCountFormatter.CountStyle

Specify the number of bytes to be used for kilobytes.

var allowsNonnumericFormatting: Bool

Determines whether to allow more natural display of some values.

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

