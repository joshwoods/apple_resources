

- WeatherKit
-  MonthPrecipitationStatistics 

Structure

# MonthPrecipitationStatistics

A structure that describes precipitation statistics for a specific month.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
struct MonthPrecipitationStatistics
```

## Topics

### Operators

static func == (MonthPrecipitationStatistics, MonthPrecipitationStatistics) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Initializers

init(from: any Decoder) throws

Creates a new instance by decoding from the given decoder.

### Instance Properties

var averagePrecipitationAmount: Measurement&lt;UnitLength>

The average amount of liquid precipitation for the month.

var averagePrecipitationProbability: Double

The average percentage probability of precipitation (0.0 = 0%, 1.0 = 100%) for the month.

var averageSnowfallAmount: Measurement&lt;UnitLength>

The average amount of snowfall as depth of snow crystals for the month.

var month: Int

The month of the year, in UTC.

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

