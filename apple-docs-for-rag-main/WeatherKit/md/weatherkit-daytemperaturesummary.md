

- WeatherKit
-  DayTemperatureSummary 

Structure

# DayTemperatureSummary

A structure that describes the temperature summary for a day.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
struct DayTemperatureSummary
```

## Topics

### Operators

static func == (DayTemperatureSummary, DayTemperatureSummary) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Initializers

init(from: any Decoder) throws

Creates a new instance by decoding from the given decoder.

### Instance Properties

var date: Date

The day of the observed temperature summary.

var highTemperature: Measurement&lt;UnitTemperature>

The observed high temperature for the day.

var lowTemperature: Measurement&lt;UnitTemperature>

The observed low temperature for the day.

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

