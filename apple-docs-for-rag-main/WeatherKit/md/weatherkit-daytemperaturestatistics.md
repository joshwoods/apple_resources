

- WeatherKit
-  DayTemperatureStatistics 

Structure

# DayTemperatureStatistics

A structure that describes temperature statistics for a day.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
struct DayTemperatureStatistics
```

## Topics

### Operators

static func == (DayTemperatureStatistics, DayTemperatureStatistics) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Initializers

init(from: any Decoder) throws

Creates a new instance by decoding from the given decoder.

### Instance Properties

var averageHighTemperature: Measurement&lt;UnitTemperature>

The average observed high temperature for the day.

var averageLowTemperature: Measurement&lt;UnitTemperature>

The average observed low temperature for the day.

var day: Int

The day of the year, in UTC.

### Instance Methods

func encode(to: any Encoder) throws

Encodes this value into the given encoder.

### Default Implementations

Equatable Implementations

## Relationships

### Conforms To

- Decodable
- Encodable
- Equatable
- Sendable

