

- WeatherKit
-  Wind 

Structure

# Wind

Contains wind data of speed, direction, and gust.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
struct Wind
```

## Topics

### Getting the properties

enum CompassDirection

A compass composed of cardinal and intercardinal directions.

var compassDirection: Wind.CompassDirection

The general indicator of wind direction.

var direction: Measurement&lt;UnitAngle>

The direction the wind is coming from in degrees.

var gust: Measurement&lt;UnitSpeed>?

A sudden increase in wind speed due to friction, wind shear, or by heating.

var speed: Measurement&lt;UnitSpeed>

Sustained wind speed.

### Default Implementations

Decodable Implementations

Encodable Implementations

Equatable Implementations

## Relationships

### Conforms To

- Copyable
- Decodable
- Encodable
- Equatable

## See Also

### Characteristics

enum Precipitation

The form of precipitation.

enum PressureTrend

The atmospheric pressure change over time.

struct UVIndex

The expected intensity of ultraviolet radiation from the sun.

enum WeatherCondition

A description of the current weather condition.

