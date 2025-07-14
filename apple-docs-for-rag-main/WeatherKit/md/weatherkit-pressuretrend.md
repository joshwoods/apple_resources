

- WeatherKit
-  PressureTrend 

Enumeration

# PressureTrend

The atmospheric pressure change over time.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
enum PressureTrend
```

## Topics

### Creating the object

init?(rawValue: String)

Creates a new instance with the specified raw value.

### Getting the trend

case falling

The pressure is falling.

case rising

The pressure is rising.

case steady

The pressure is not changing.

### Describing the trend

var accessibilityDescription: String

A localized accessibility description describing the pressure change over time.

var description: String

A localized string describing the pressure trend.

### Instance Properties

var rawValue: String

The corresponding value of the raw type.

### Type Aliases

typealias AllCases

A type that can represent a collection of all values of this type.

typealias RawValue

The raw type that can be used to represent all values of the conforming type.

### Type Properties

static var allCases: [PressureTrend]

A collection of all values of this type.

### Default Implementations

Equatable Implementations

RawRepresentable Implementations

## Relationships

### Conforms To

- CaseIterable
- Copyable
- CustomStringConvertible
- Decodable
- Encodable
- Equatable
- Hashable
- RawRepresentable

## See Also

### Characteristics

enum Precipitation

The form of precipitation.

struct UVIndex

The expected intensity of ultraviolet radiation from the sun.

struct Wind

Contains wind data of speed, direction, and gust.

enum WeatherCondition

A description of the current weather condition.

