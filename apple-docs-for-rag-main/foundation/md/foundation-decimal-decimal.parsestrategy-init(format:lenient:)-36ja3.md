

- Foundation
- Decimal
- Decimal.ParseStrategy
-  init(format:lenient:) 

Initializer

# init(format:lenient:)

Creates a parse strategy instance using the specified decimal percentage format style.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
init(
    format: Format,
    lenient: Bool = true
)
```

Available when `Format` is `Decimal.FormatStyle.Percent`.

## Parameters 

`format`  

A configured Decimal.FormatStyle that describes the percent string format to parse.

`lenient`  

A Boolean value that indicates whether the parse strategy should permit some discrepencies when parsing. Defaults to `true`.

## See Also

### Creating a decimal parse strategy

init(format: Format, lenient: Bool)

Creates a parse strategy instance using the specified decimal format style.

init(format: Format, lenient: Bool)

Creates a parse strategy instance using the specified decimal currency format style.

