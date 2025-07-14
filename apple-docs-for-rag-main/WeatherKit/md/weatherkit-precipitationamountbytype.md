

- WeatherKit
-  PrecipitationAmountByType 

Structure

# PrecipitationAmountByType

A structure that provides a breakdown of amounts of all forms of precipitation that is expected to occur over a period of time.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
struct PrecipitationAmountByType
```

## Topics

### Operators

static func == (PrecipitationAmountByType, PrecipitationAmountByType) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Initializers

init(from: any Decoder) throws

Creates a new instance by decoding from the given decoder.

### Instance Properties

var hail: Measurement&lt;UnitLength>

The amount of hail for the period.

var mixed: Measurement&lt;UnitLength>

The amount of wintry mix for the period.

var precipitation: Measurement&lt;UnitLength>

The amount of liquid equivalent of all precipitation for the period.

var rainfall: Measurement&lt;UnitLength>

The amount of rainfall for the period.

var sleet: Measurement&lt;UnitLength>

The amount of sleet for the period.

var snowfallAmount: SnowfallAmount

Describes the amount of snowfall for the period.

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

