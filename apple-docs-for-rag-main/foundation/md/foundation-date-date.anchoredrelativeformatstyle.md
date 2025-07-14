

- Foundation
- Date
-  Date.AnchoredRelativeFormatStyle 

Structure

# Date.AnchoredRelativeFormatStyle

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 1.0+watchOS 11.0+

``` source
struct AnchoredRelativeFormatStyle
```

## Topics

### Initializers

init(anchor: Date, allowedFields: Set&lt;Date.AnchoredRelativeFormatStyle.Field>, presentation: Date.AnchoredRelativeFormatStyle.Presentation, unitsStyle: Date.AnchoredRelativeFormatStyle.UnitsStyle, locale: Locale, calendar: Calendar, capitalizationContext: FormatStyleCapitalizationContext)

init(anchor: Date, presentation: Date.AnchoredRelativeFormatStyle.Presentation, unitsStyle: Date.AnchoredRelativeFormatStyle.UnitsStyle, locale: Locale, calendar: Calendar, capitalizationContext: FormatStyleCapitalizationContext)

### Instance Properties

var allowedFields: Set&lt;Date.AnchoredRelativeFormatStyle.Field>

var anchor: Date

var calendar: Calendar

var capitalizationContext: FormatStyleCapitalizationContext

var locale: Locale

var presentation: Date.AnchoredRelativeFormatStyle.Presentation

var unitsStyle: Date.AnchoredRelativeFormatStyle.UnitsStyle

### Type Aliases

typealias Field

typealias Presentation

typealias UnitsStyle

## Relationships

### Conforms To

- Copyable
- Decodable
- DiscreteFormatStyle
- Encodable
- Equatable
- FormatStyle
- Hashable
- Sendable

