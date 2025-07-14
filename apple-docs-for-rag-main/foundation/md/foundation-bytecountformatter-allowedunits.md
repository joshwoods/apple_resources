

- Foundation
- ByteCountFormatter
-  allowedUnits 

Instance Property

# allowedUnits

Specify the units that can be used in the output.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+macOS 10.8+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var allowedUnits: ByteCountFormatter.Units { get set }
```

## Discussion

If the value is NSByteCountFormatterUseDefault, the formatter uses platform-appropriate settings; otherwise will only the specified units are used.

ByteCountFormatter.Units values can be combined using the C `OR` operator to specify complex formatting strings. The NSByteCountFormatterUseDefault or useAll constants can be used with the C `AND` or the C `NOT` operators to create custom formats as well.

This is the default value if NSByteCountFormatterUseDefault.

Note

ZB and YB cannot be covered by the range of possible values, but you can still choose to use these units to get fractional display (`0.0035 ZB` for instance).

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

var includesCount: Bool

Determines whether to include the count in the resulting formatted string.

var includesUnit: Bool

Determines whether to include the units in the resulting formatted string.

var zeroPadsFractionDigits: Bool

Determines whether to zero pad fraction digits so a consistent number of characters is displayed in a representation.

