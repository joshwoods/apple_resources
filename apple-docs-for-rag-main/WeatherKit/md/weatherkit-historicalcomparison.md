

- WeatherKit
-  HistoricalComparison 

Enumeration

# HistoricalComparison

An enum that represents a recognized comparison in the statistical analysis of a location’s historical weather data.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
enum HistoricalComparison
```

## Topics

### Operators

static func == (HistoricalComparison, HistoricalComparison) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Enumeration Cases

case highTemperature(Trend&lt;UnitTemperature>)

The comparison relates to the location’s maximum temperature averaged since ~1970.

case lowTemperature(Trend&lt;UnitTemperature>)

The comparison relates to the location’s minimum temperature averaged since ~1970.

case precipitationAmount(Trend&lt;UnitLength>)

The comparison relates to the amount of precipitation at the location averaged over the past 30 days.

case snowfallAmount(Trend&lt;UnitLength>)

The comparison relates to the amount of snowfall at the location averaged over the past 30 days.

### Initializers

init(from: any Decoder) throws

Creates a new instance by decoding from the given decoder.

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

