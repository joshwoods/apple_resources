

- WeatherKit
-  DayPrecipitationStatistics 

Structure

# DayPrecipitationStatistics

A structure that describes precipitation statistics for a day.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
struct DayPrecipitationStatistics
```

## Topics

### Operators

static func == (DayPrecipitationStatistics, DayPrecipitationStatistics) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Initializers

init(from: any Decoder) throws

Creates a new instance by decoding from the given decoder.

### Instance Properties

var averagePrecipitationAmount: Measurement&lt;UnitLength>

The average amount of liquid precipitation for the day.

var averagePrecipitationProbability: Double

The average percentage probability of precipitation (0.0 = 0%, 1.0 = 100%) for the day.

var averageSnowfallAmount: Measurement&lt;UnitLength>

The average amount of snowfall as depth of snow crystals for the day.

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

