

- WeatherKit
-  WeatherSeverity 

Enumeration

# WeatherSeverity

A description of the severity of the severe weather event.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
enum WeatherSeverity
```

## Topics

### Creating the object

init?(rawValue: String)

Creates a new instance with the specified raw value.

### Getting the properties

case minor

Minimal or no known threat.

case moderate

Possible threat.

case severe

Significant threat.

case extreme

Extraordinary threat.

case unknown

Unknown threat.

### Describing the weather severity

var accessibilityDescription: String

A localized accessibility description describing the weather severity.

var description: String

A localized string describing the weather severity.

### Instance Properties

var rawValue: String

The corresponding value of the raw type.

### Type Aliases

typealias AllCases

A type that can represent a collection of all values of this type.

typealias RawValue

The raw type that can be used to represent all values of the conforming type.

### Type Properties

static var allCases: [WeatherSeverity]

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

### Requests

struct WeatherQuery

A structure that encapsulates a generic weather dataset request.

struct CurrentWeather

A structure that describes the current conditions observed at a location.

struct WeatherAttribution

A structure that defines the necessary information for attributing a weather data provider.

struct WeatherMetadata

A structure that provides additional weather information.

