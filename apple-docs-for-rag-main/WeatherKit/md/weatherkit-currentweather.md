

- WeatherKit
-  CurrentWeather 

Structure

# CurrentWeather

A structure that describes the current conditions observed at a location.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
struct CurrentWeather
```

## Overview

The current conditions may not be a literal observation, but rather the result of a mathematical weather model predicting conditions based on real observations.

## Topics

### Getting temperature and humidity

var apparentTemperature: Measurement&lt;UnitTemperature>

The feels-like temperature when factoring wind and humidity.

var dewPoint: Measurement&lt;UnitTemperature>

The temperature at which relative humidity is 100%.

var humidity: Double

The amount of water vapor in the air.

var temperature: Measurement&lt;UnitTemperature>

The current temperature.

### Getting wind and pressure

var pressure: Measurement&lt;UnitPressure>

The sea level air pressure in millibars.

var pressureTrend: PressureTrend

The direction of change of the sea level air pressure.

var wind: Wind

The wind speed, direction, and gust.

### Getting conditions

var cloudCover: Double

The percentage of the sky covered with clouds.

var condition: WeatherCondition

An enumeration value indicating the condition at the time.

### Getting date and validity

var date: Date

The date of the current weather.

### Getting daylight and visibility

var isDaylight: Bool

A Boolean value indicating whether there is daylight.

var uvIndex: UVIndex

The level of ultraviolet radiation.

var visibility: Measurement&lt;UnitLength>

The distance at which terrain is visible.

### Getting additional information

var metadata: WeatherMetadata

Descriptive information about the current weather data.

var symbolName: String

The SF Symbol icon that represents the current weather condition and whether it’s daylight at the current date.

### Instance Properties

var cloudCoverByAltitude: CloudCoverByAltitude

The percentage of the sky covered with low-altitude, middle altitude and high-altitude clouds during the period.

var precipitationIntensity: Measurement&lt;UnitSpeed>

The current precipitation intensity in kilometers per hour.

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

### Requests

struct WeatherQuery

A structure that encapsulates a generic weather dataset request.

struct WeatherAttribution

A structure that defines the necessary information for attributing a weather data provider.

struct WeatherMetadata

A structure that provides additional weather information.

enum WeatherSeverity

A description of the severity of the severe weather event.

