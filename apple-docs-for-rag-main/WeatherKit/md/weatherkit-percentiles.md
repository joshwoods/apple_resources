

- WeatherKit
-  Percentiles 

Structure

# Percentiles

A structure that describes probability distributions for a measurable weather condition.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
struct Percentiles where Dimension : Dimension
```

## Topics

### Operators

static func == (Percentiles&lt;Dimension>, Percentiles&lt;Dimension>) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Initializers

init(from: any Decoder) throws

Creates a new instance by decoding from the given decoder.

### Instance Properties

var p10: Measurement&lt;Dimension>

10% of the distribution is less than this value.

var p50: Measurement&lt;Dimension>

50% of the distribution is less than this value.

var p90: Measurement&lt;Dimension>

90% of the distribution is less than this value.

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

