

- WeatherKit
-  HourTemperatureStatistics 

Structure

# HourTemperatureStatistics

A structure that describes temperature statistics for a specific hour.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
struct HourTemperatureStatistics
```

## Topics

### Operators

static func == (HourTemperatureStatistics, HourTemperatureStatistics) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Initializers

init(from: any Decoder) throws

Creates a new instance by decoding from the given decoder.

### Instance Properties

var hour: Int

The hour of the year, in UTC.

var percentiles: Percentiles&lt;UnitTemperature>

The temperature statistics for the hour.

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

