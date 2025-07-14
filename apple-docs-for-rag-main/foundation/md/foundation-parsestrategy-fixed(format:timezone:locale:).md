

- Foundation
- ParseStrategy
-  fixed(format:timeZone:locale:) 

Type Method

# fixed(format:timeZone:locale:)

A fixed-format date parse strategy.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
static func fixed(
    format: Date.FormatString,
    timeZone: TimeZone,
    locale: Locale? = nil
) -> Self where Self == Date.ParseStrategy
```

## Parameters 

`format`  

The string describing the parsing format.

`timeZone`  

The TimeZone used to create the string representation of the date.

`locale`  

The Locale used to create the string representation of the date.

## Return Value

A strategy for parsing a date.

## See Also

### Commonly-used parsers

static var url: URL.ParseStrategy

A parse strategy for URLs.

static var name: PersonNameComponents.ParseStrategy

A parse strategy for person name components.

