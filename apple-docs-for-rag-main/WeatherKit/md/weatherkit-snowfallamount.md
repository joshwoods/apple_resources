

- WeatherKit
-  SnowfallAmount 

Structure

# SnowfallAmount

A structure that describes the snowfall amount over a period of time.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
struct SnowfallAmount
```

## Topics

### Operators

static func == (SnowfallAmount, SnowfallAmount) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Initializers

init(from: any Decoder) throws

Creates a new instance by decoding from the given decoder.

### Instance Properties

var amount: Measurement&lt;UnitLength>

The estimated amount of snowfall as depth of snow crystals for the period.

var amountLiquidEquivalent: Measurement&lt;UnitLength>

The estimated amount of snowfall as liquid equivalent for the period.

var maximum: Measurement&lt;UnitLength>

The maximum amount of snowfall as depth of snow crystals for the period.

var maximumLiquidEquivalent: Measurement&lt;UnitLength>

The maximum amount of snowfall as liquid equivalent for the period.

var minimum: Measurement&lt;UnitLength>

The minimum amount of snowfall as depth of snow crystals for the period.

var minimumLiquidEquivalent: Measurement&lt;UnitLength>

The minimum amount of snowfall as liquid equivalent for the period.

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

