

- Foundation
- ParseStrategy
-  name 

Type Property

# name

A parse strategy for person name components.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
static var name: PersonNameComponents.ParseStrategy { get }
```

Available when `Self` is `PersonNameComponents.ParseStrategy`.

## See Also

### Commonly-used parsers

static func fixed(format: Date.FormatString, timeZone: TimeZone, locale: Locale?) -> Self

A fixed-format date parse strategy.

static var url: URL.ParseStrategy

A parse strategy for URLs.

