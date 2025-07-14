

- Foundation
- Decimal
-  init(\_:format:lenient:) 

Initializer

# init(\_:format:lenient:)

Creates and initializes a decimal by parsing a string according to the provided format style.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
init(
    _ value: String,
    format: Decimal.FormatStyle,
    lenient: Bool = true
) throws
```

## Parameters 

`value`  

A string that contains a formatted decimal value.

`format`  

A format style that describes formatting conventions used by the string. The initializer uses this format’s `Decimal/FormatStyle/parseStrategy` to parse the string.

`lenient`  

A Boolean value that indicates whether the parse strategy should permit some discrepancies when parsing. Defaults to `true`.

## Discussion

This initializer throws an error if the format style fails to parse the string into a decimal value.

## See Also

### Creating a decimal by parsing a string

init(String, format: Decimal.FormatStyle.Currency, lenient: Bool) throws

Creates and initializes a decimal by parsing a string according to the provided currency format style.

init(String, format: Decimal.FormatStyle.Percent, lenient: Bool) throws

Creates and initializes a percentage decimal by parsing a string according to the provided format style.

init?(string: String, locale: Locale?)

Creates and initializes a decimal by parsing a string according to the provided locale’s conventions.

init&lt;S>(S.ParseInput, strategy: S) throws

Creates and initializes a decimal by parsing an arbitrary type according to the provided parse strategy.

struct ParseStrategy

A parse strategy for creating decimal values from formatted strings.

