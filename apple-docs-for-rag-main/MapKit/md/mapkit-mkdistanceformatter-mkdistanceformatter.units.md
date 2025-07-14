

- MapKit
- MKDistanceFormatter
-  MKDistanceFormatter.Units 

Enumeration

# MKDistanceFormatter.Units

Constants that reflect the type of units to use in the string.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.2+visionOS 1.0+watchOS 2.0+

``` source
enum Units
```

## Topics

### Constants

case `default`

The format uses the locale information to determine which units to use.

case metric

The format uses metric units.

case imperial

The format uses imperial units.

case imperialWithYards

The format uses imperial units that include measurements in yards.

case `default`

The format uses the locale information to determine which units to use.

case metric

The format uses metric units.

case imperial

The format uses imperial units.

case imperialWithYards

The format uses imperial units that include measurements in yards.

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

var unitStyle: MKDistanceFormatter.DistanceUnitStyle

The preferred style for units.

enum DistanceUnitStyle

Constants that indicate the format style to use for strings.

