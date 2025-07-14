

- WeatherKit
-  Deviation 

Enumeration

# Deviation

Describes a comparison between two values in a trend.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
enum Deviation
```

## Topics

### Operators

static func == (Deviation, Deviation) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Enumeration Cases

case higher

The most recently observed value is larger than the value it is being compared against.

case lower

The most recently observed value is lower than the value it is being compared against.

case muchHigher

The most recently observed value is much larger than the value it is being compared against.

case muchLower

The most recently observed value is much lower than the value it is being compared against.

case normal

The most recently observed value is about the same as the value it is being compared against.

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

