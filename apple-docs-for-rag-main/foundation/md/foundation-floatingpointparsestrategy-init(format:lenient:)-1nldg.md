

- Foundation
- FloatingPointParseStrategy
-  init(format:lenient:) 

Initializer

# init(format:lenient:)

Creates a parse strategy instance using the specified floating-point percentage format style.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
init(
    format: Format,
    lenient: Bool = true
) where Format == FloatingPointFormatStyle.Percent, Value : BinaryFloatingPoint
```

Available when `Format` conforms to `FormatStyle` and `Format.FormatInput` conforms to `BinaryFloatingPoint`.

## Parameters 

`format`  

A configured FloatingPointFormatStyle.Percent that describes the percent string format to parse.

`lenient`  

A Boolean value that indicates whether the parse strategy should permit some discrepencies when parsing. Defaults to `true`.

## See Also

### Creating a floating-point parse strategy

init&lt;Value>(format: Format, lenient: Bool)

Creates a parse strategy instance using the specified floating-point format style.

init&lt;Value>(format: Format, lenient: Bool)

Creates a parse strategy instance using the specified floating-point currency format style.

