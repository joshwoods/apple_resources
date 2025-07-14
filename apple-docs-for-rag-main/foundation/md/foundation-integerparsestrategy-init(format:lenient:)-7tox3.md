

- Foundation
- IntegerParseStrategy
-  init(format:lenient:) 

Initializer

# init(format:lenient:)

Creates a parse strategy instance using the specified integer currency format style.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
init(
    format: Format,
    lenient: Bool = true
) where Format == IntegerFormatStyle.Currency, Value : BinaryInteger
```

Available when `Format` conforms to `FormatStyle` and `Format.FormatInput` conforms to `BinaryInteger`.

## Parameters 

`format`  

A configured IntegerFormatStyle.Currency that describes the currency string format to parse.

`lenient`  

A Boolean value that indicates whether the parse strategy should permit some discrepencies when parsing. Defaults to `true`.

## See Also

### Creating an integer parse strategy

init&lt;Value>(format: Format, lenient: Bool)

Creates a parse strategy instance using the specified integer format style.

init&lt;Value>(format: Format, lenient: Bool)

Creates a parse strategy instance using the specified integer percentage format style.

