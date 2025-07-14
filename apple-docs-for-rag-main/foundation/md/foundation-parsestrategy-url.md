

- Foundation
- ParseStrategy
-  url 

Type Property

# url

A parse strategy for URLs.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
static var url: URL.ParseStrategy { get }
```

Available when `Self` is `URL.ParseStrategy`.

## Discussion

Use the dot-notation form of this type property when the call point allows the use of URL.ParseStrategy. Typically, you use this with the URL initializer init(_:strategy:).

## See Also

### Commonly-used parsers

static func fixed(format: Date.FormatString, timeZone: TimeZone, locale: Locale?) -> Self

A fixed-format date parse strategy.

static var name: PersonNameComponents.ParseStrategy

A parse strategy for person name components.

