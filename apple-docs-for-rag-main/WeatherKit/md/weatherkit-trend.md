

- WeatherKit
-  Trend 

Structure

# Trend

A structure describing an observed pattern in the data for weather at a location for a specific condition.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
struct Trend where Dimension : Dimension
```

## Topics

### Operators

static func == (Trend&lt;Dimension>, Trend&lt;Dimension>) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Initializers

init(from: any Decoder) throws

Creates a new instance by decoding from the given decoder.

### Instance Properties

var baseline: TrendBaseline&lt;Dimension>

The manner in which the comparison between the baseline and current values are compared.

var currentValue: Measurement&lt;Dimension>

The current recorded value for the condition in which the trend is compared against.

var deviation: Deviation

Semantically describes the manner in which the observed trend compares the current value against the baseline value.

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

