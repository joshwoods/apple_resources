

- WeatherKit
- TrendBaseline
-  TrendBaseline.Kind 

Enumeration

# TrendBaseline.Kind

An enum describing what value is being compared between historical and current readings.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
enum Kind
```

## Topics

### Operators

static func == (TrendBaseline&lt;Dimension>.Kind, TrendBaseline&lt;Dimension>.Kind) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Enumeration Cases

case mean

The baseline value is a mean (or average) of other values.

### Initializers

init(from: any Decoder) throws

Creates a new instance by decoding from the given decoder.

### Instance Properties

var hashValue: Int

The hash value.

### Instance Methods

func encode(to: any Encoder) throws

Encodes this value into the given encoder.

func hash(into: inout Hasher)

Hashes the essential components of this value by feeding them into the given hasher.

### Default Implementations

Equatable Implementations

## Relationships

### Conforms To

- Copyable
- Decodable
- Encodable
- Equatable
- Hashable

