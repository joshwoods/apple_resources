

- Foundation
- ByteCountFormatter
-  isAdaptive 

Instance Property

# isAdaptive

Determines the display style of the size representation.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+macOS 10.8+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var isAdaptive: Bool { get set }
```

## Discussion

The “adaptive” algorithm is platform specific and uses a different number of fraction digits based on the magnitude (in OS X v10.8: 0 fraction digits for bytes and KB; 1 fraction digits for MB; 2 for GB and above). Otherwise the result always tries to show at least three significant digits, introducing fraction digits as necessary.

Default is true.

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

var allowedUnits: ByteCountFormatter.Units

Specify the units that can be used in the output.

var includesCount: Bool

Determines whether to include the count in the resulting formatted string.

var includesUnit: Bool

Determines whether to include the units in the resulting formatted string.

var zeroPadsFractionDigits: Bool

Determines whether to zero pad fraction digits so a consistent number of characters is displayed in a representation.

