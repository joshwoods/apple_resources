

- Foundation
- ByteCountFormatter
-  zeroPadsFractionDigits 

Instance Property

# zeroPadsFractionDigits

Determines whether to zero pad fraction digits so a consistent number of characters is displayed in a representation.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+macOS 10.8+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var zeroPadsFractionDigits: Bool { get set }
```

## Discussion

Displaying values using zero pad fraction digits causes a consistent number of fraction digits are displayed, causing updating displays to remain more stable. For instance, if the isAdaptive algorithm is used, this option formats 1.19 and 1.2 GB as `1.19 GB` and `1.20 GB`, respectively, while without the option the latter would be displayed as `1.2 GB`.

The default value is false.

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

var includesUnit: Bool

Determines whether to include the units in the resulting formatted string.

