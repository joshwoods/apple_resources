

- MapKit
- MKDistanceFormatter
-  MKDistanceFormatter.DistanceUnitStyle 

Enumeration

# MKDistanceFormatter.DistanceUnitStyle

Constants that indicate the format style to use for strings.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.2+visionOS 1.0+watchOS 2.0+

``` source
enum DistanceUnitStyle
```

## Topics

### Constants

case `default`

Bases the determination to abbreviate on the current locale and user language settings.

case abbreviated

Abbreviates units.

case full

Spells out units in full.

case `default`

Bases the determination to abbreviate on the current locale and user language settings.

case abbreviated

Abbreviates units.

case full

Spells out units in full.

### Initializers

init?(rawValue: UInt)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Specifying the format

var locale: Locale!

The locale to use when formatting strings.

var units: MKDistanceFormatter.Units

The measuring system — imperial or metric — to use for units.

enum Units

Constants that reflect the type of units to use in the string.

var unitStyle: MKDistanceFormatter.DistanceUnitStyle

The preferred style for units.

