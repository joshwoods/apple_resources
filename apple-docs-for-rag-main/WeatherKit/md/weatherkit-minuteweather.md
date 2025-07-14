

- WeatherKit
-  MinuteWeather 

Structure

# MinuteWeather

A structure that represents the next hour minute forecasts.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
struct MinuteWeather
```

## Topics

### Getting the precipitation

var precipitation: Precipitation

A description of the precipitation for this minute.

var precipitationChance: Double

The probability of precipitation in this minute.

var precipitationIntensity: Measurement&lt;UnitSpeed>

The forecasted precipitation intensity.

### Getting the date

var date: Date

The start time of the minute weather.

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

struct HourWeather

A structure that represents the weather conditions for the hour.

struct DayWeather

A structure that represents the weather conditions for the day.

