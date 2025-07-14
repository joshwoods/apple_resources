

- WeatherKit
- Weather
-  minuteForecast 

Instance Property

# minuteForecast

The minute-by-minute forecast.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
var minuteForecast: Forecast?
```

## Discussion

Depending upon region support and data availability, this may be `nil`.

## See Also

### Getting the forecast

var availability: WeatherAvailability

Flags containing information about data availability and attribution.

var currentWeather: CurrentWeather

The current weather forecast.

var dailyForecast: Forecast&lt;DayWeather>

The daily forecast.

var hourlyForecast: Forecast&lt;HourWeather>

The hourly forecast.

