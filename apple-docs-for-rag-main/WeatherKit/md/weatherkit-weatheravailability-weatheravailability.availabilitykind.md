

- WeatherKit
- WeatherAvailability
-  WeatherAvailability.AvailabilityKind 

Enumeration

# WeatherAvailability.AvailabilityKind

The availability kind.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
enum AvailabilityKind
```

## Topics

### Enumeration Cases

case available

The data is available.

case temporarilyUnavailable

The data is supported for the location but is temporarily unavailable.

case unknown

The availability is unknown.

case unsupported

The data isn’t supported for the location.

### Initializers

init?(rawValue: String)

Creates a new instance with the specified raw value.

### Instance Properties

var rawValue: String

The corresponding value of the raw type.

### Type Aliases

typealias RawValue

The raw type that can be used to represent all values of the conforming type.

### Default Implementations

Equatable Implementations

RawRepresentable Implementations

## Relationships

### Conforms To

- Copyable
- Decodable
- Encodable
- Equatable
- Hashable
- RawRepresentable

## See Also

### Getting the properties

var alertAvailability: WeatherAvailability.AvailabilityKind

The weather alerts availability.

var minuteAvailability: WeatherAvailability.AvailabilityKind

The minute forecast availability.

