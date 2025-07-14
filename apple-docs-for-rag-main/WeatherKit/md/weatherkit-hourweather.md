

- WeatherKit
-  HourWeather 

Structure

# HourWeather

A structure that represents the weather conditions for the hour.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
struct HourWeather
```

## Topics

### Getting temperature and humidity

var apparentTemperature: Measurement&lt;UnitTemperature>

The apparent, or “feels like” temperature during the hour.

var humidity: Double

The humidity for the hour.

var temperature: Measurement&lt;UnitTemperature>

The temperature during the hour.

var dewPoint: Measurement&lt;UnitTemperature>

The amount of moisture in the air.

### Getting pressure

var pressure: Measurement&lt;UnitPressure>

The atmospheric pressure at sea level at a given location.

var pressureTrend: PressureTrend

The kind and amount of atmospheric pressure change over time.

### Getting conditions

var cloudCover: Double

The percentage of the sky covered with clouds.

var condition: WeatherCondition

A description of the weather condition for this hour.

var isDaylight: Bool

The presence or absence of daylight at the requested location and hour.

var visibility: Measurement&lt;UnitLength>

The distance at which an object can be clearly seen.

### Getting the UV index

var uvIndex: UVIndex

The expected intensity of ultraviolet radiation from the sun.

### Getting the wind

var wind: Wind

Wind data describing the wind speed, direction, and gust.

### Getting the date

var date: Date

The start time of the hour weather.

### Getting the precipitation

var precipitation: Precipitation

Description of precipitation for this hour.

var precipitationChance: Double

The probability of precipitation during the hour.

### Getting the weather symbol

var symbolName: String

The SF Symbol icon that represents the hour weather condition and whether it’s daylight on the hour.

### Instance Properties

var cloudCoverByAltitude: CloudCoverByAltitude

The percentage of the sky covered with low altitude, middle altitude and high altitude clouds during the period.

var precipitationAmount: Measurement&lt;UnitLength>

The amount of precipitation for the hour.

var snowfallAmount: Measurement&lt;UnitLength>

The amount of snowfall for the hour.

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

### Alerts and forecasts

struct WeatherAlert

A weather alert issued for the requested location by a governmental authority.

struct WeatherAvailability

A structure that indicates the availability of data at the requested location.

struct Forecast

A forecast collection for minute, hourly, and daily forecasts.

struct MinuteWeather

A structure that represents the next hour minute forecasts.

struct DayWeather

A structure that represents the weather conditions for the day.

