

- WeatherKit
-  Weather 

Structure

# Weather

A model representing the aggregate weather data the caller requests.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
struct Weather
```

## Topics

### Getting the forecast

var availability: WeatherAvailability

Flags containing information about data availability and attribution.

var currentWeather: CurrentWeather

The current weather forecast.

var dailyForecast: Forecast&lt;DayWeather>

The daily forecast.

var hourlyForecast: Forecast&lt;HourWeather>

The hourly forecast.

var minuteForecast: Forecast&lt;MinuteWeather>?

The minute-by-minute forecast.

### Getting weather alerts

var weatherAlerts: [WeatherAlert]?

A list of severe weather alerts.

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

### Fundamentals

Fetching weather forecasts with WeatherKit

Request and display weather data for destination airports in a flight-planning app.

class WeatherService

Provides an interface for obtaining weather data.

