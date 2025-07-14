

- WeatherKit
-  DayWeather 

Structure

# DayWeather

A structure that represents the weather conditions for the day.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
struct DayWeather
```

## Topics

### Getting temperature

var highTemperature: Measurement&lt;UnitTemperature>

The daytime high temperature.

var lowTemperature: Measurement&lt;UnitTemperature>

The overnight low temperature.

### Getting precipitation

var precipitation: Precipitation

The description of precipitation for this day.

var precipitationChance: Double

The probability of precipitation during the day.

var rainfallAmount: Measurement&lt;UnitLength>

The amount of liquid precipitation for the day.

Deprecated

var snowfallAmount: Measurement&lt;UnitLength>

The amount of snowfall for the day.

Deprecated

### Getting celestial information

var moon: MoonEvents

The lunar events for the day.

var sun: SunEvents

The solar events for the day.

### Getting the wind

var wind: Wind

The wind speed, direction, and gust.

### Getting the date

var date: Date

The start time of the day weather.

### Getting condition and UV index

var condition: WeatherCondition

A description of the weather condition on this day.

var uvIndex: UVIndex

The expected intensity of ultraviolet radiation from the sun.

### Getting the weather symbol

var symbolName: String

The SF Symbol icon that represents the day weather condition.

### Instance Properties

var daytimeForecast: DayPartForecast

The weather forecast from 7AM - 7PM on this day.

var highTemperatureTime: Date?

The time at which the high temperature occurs on this day.

var highWindSpeed: Measurement&lt;UnitSpeed>?

The maximum sustained wind speed.

var lowTemperatureTime: Date?

The time at which the low temperature occurs on this day.

var maximumHumidity: Double

The maximum amount of water vapor in the air for the day.

var maximumVisibility: Double

The maximum distance, in meters, at which terrain is visible for the day.

var minimumHumidity: Double

The minimum amount of water vapor in the air for the day.

var minimumVisibility: Double

The minimum distance, in meters, at which terrain is visible for the day.

var overnightForecast: DayPartForecast

The weather forecast for 7PM on this day until 7AM the following day.

var precipitationAmount: Measurement&lt;UnitLength>

The amount of liquid precipitation for the day.

Deprecated

var precipitationAmountByType: PrecipitationAmountByType

A breakdown of amounts of all forms of precipitation forecasted for the day.

var restOfDayForecast: DayPartForecast?

The forecast from now until midnight local time.

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

struct HourWeather

A structure that represents the weather conditions for the hour.

