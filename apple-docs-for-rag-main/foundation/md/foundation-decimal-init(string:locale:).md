

- Foundation
- Decimal
-  init(string:locale:) 

Initializer

# init(string:locale:)

Creates and initializes a decimal by parsing a string according to the provided locale’s conventions.

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
init?(
    string: String,
    locale: Locale? = nil
)
```

## Parameters 

`string`  

A string containing a formatted decimal value.

`locale`  

A locale that indicates the formatting conventions used by `string`.

## See Also

### Creating a decimal by parsing a string

init(String, format: Decimal.FormatStyle, lenient: Bool) throws

Creates and initializes a decimal by parsing a string according to the provided format style.

init(String, format: Decimal.FormatStyle.Currency, lenient: Bool) throws

Creates and initializes a decimal by parsing a string according to the provided currency format style.

init(String, format: Decimal.FormatStyle.Percent, lenient: Bool) throws

Creates and initializes a percentage decimal by parsing a string according to the provided format style.

init&lt;S>(S.ParseInput, strategy: S) throws

Creates and initializes a decimal by parsing an arbitrary type according to the provided parse strategy.

struct ParseStrategy

A parse strategy for creating decimal values from formatted strings.

