

- Foundation
- Decimal
-  init(\_:strategy:) 

Initializer

# init(\_:strategy:)

Creates and initializes a decimal by parsing an arbitrary type according to the provided parse strategy.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
init(
    _ value: S.ParseInput,
    strategy: S
) throws where S : ParseStrategy, S.ParseOutput == Decimal
```

## Parameters 

`value`  

An instance of `strategy`’s input type.

`strategy`  

A parse strategy that describes how the parser converts the string to a decimal value.

## See Also

### Creating a decimal by parsing a string

init(String, format: Decimal.FormatStyle, lenient: Bool) throws

Creates and initializes a decimal by parsing a string according to the provided format style.

init(String, format: Decimal.FormatStyle.Currency, lenient: Bool) throws

Creates and initializes a decimal by parsing a string according to the provided currency format style.

init(String, format: Decimal.FormatStyle.Percent, lenient: Bool) throws

Creates and initializes a percentage decimal by parsing a string according to the provided format style.

init?(string: String, locale: Locale?)

Creates and initializes a decimal by parsing a string according to the provided locale’s conventions.

struct ParseStrategy

A parse strategy for creating decimal values from formatted strings.

