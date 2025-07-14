

- WeatherKit
- WeatherChange
-  WeatherChange.Direction 

Enumeration

# WeatherChange.Direction

An enum that specifies the direction in which a measurable aspect of the weather is expected to change.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
@frozen
enum Direction
```

## Topics

### Enumeration Cases

case decrease

The value will be significantly lower than before.

case increase

The value will be significantly higher than before.

case steady

The value will remain similar to before.

### Instance Properties

var hashValue: Int

The hash value.

### Instance Methods

func hash(into: inout Hasher)

Hashes the essential components of this value by feeding them into the given hasher.

### Default Implementations

Decodable Implementations

Encodable Implementations

Equatable Implementations

## Relationships

### Conforms To

- BitwiseCopyable
- Copyable
- Decodable
- Encodable
- Equatable
- Hashable
- Sendable

