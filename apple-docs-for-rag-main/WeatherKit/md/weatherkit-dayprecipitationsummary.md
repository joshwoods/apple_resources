

- WeatherKit
-  DayPrecipitationSummary 

Structure

# DayPrecipitationSummary

A structure that describes the precipitation summary for a day.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
struct DayPrecipitationSummary
```

## Topics

### Operators

static func == (DayPrecipitationSummary, DayPrecipitationSummary) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Initializers

init(from: any Decoder) throws

Creates a new instance by decoding from the given decoder.

### Instance Properties

var date: Date

The day of the observed precipitation summary

var precipitationAmount: Measurement&lt;UnitLength>

The amount of liquid precipitation for the day.

var snowfallAmount: Measurement&lt;UnitLength>

The snowfall amount as depth of snow crystals for the day.

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

