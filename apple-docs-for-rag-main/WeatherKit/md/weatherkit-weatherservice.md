

- WeatherKit
-  WeatherService 

Class

# WeatherService

Provides an interface for obtaining weather data.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
final class WeatherService
```

## Topics

### Creating the object

convenience init()

Creates a weather service object.

### Obtaining forecasts

func weather(for: CLLocation) async throws -> Weather

Returns the weather forecast for the requested location.

func weather&lt;T1, T2>(for: CLLocation, including: WeatherQuery&lt;T1>, WeatherQuery&lt;T2>) async throws -> (T1, T2)

Returns the weather forecast for the requested location.

func weather&lt;T1, T2, T3>(for: CLLocation, including: WeatherQuery&lt;T1>, WeatherQuery&lt;T2>, WeatherQuery&lt;T3>) async throws -> (T1, T2, T3)

Returns the weather forecast for the requested location.

func weather&lt;T1, T2, T3, T4>(for: CLLocation, including: WeatherQuery&lt;T1>, WeatherQuery&lt;T2>, WeatherQuery&lt;T3>, WeatherQuery&lt;T4>) async throws -> (T1, T2, T3, T4)

Returns the weather forecast for the requested location.

func weather&lt;T1, T2, T3, T4, T5>(for: CLLocation, including: WeatherQuery&lt;T1>, WeatherQuery&lt;T2>, WeatherQuery&lt;T3>, WeatherQuery&lt;T4>, WeatherQuery&lt;T5>) async throws -> (T1, T2, T3, T4, T5)

Returns the weather forecast for the requested location.

func weather&lt;T1, T2, T3, T4, T5, T6>(for: CLLocation, including: WeatherQuery&lt;T1>, WeatherQuery&lt;T2>, WeatherQuery&lt;T3>, WeatherQuery&lt;T4>, WeatherQuery&lt;T5>, WeatherQuery&lt;T6>) async throws -> (T1, T2, T3, T4, T5, T6)

Returns the weather forecast for the requested location.

static let shared: WeatherService

A single, shared weather service object.

### Providing attribution

var attribution: WeatherAttribution

The required attribution which includes a legal attribution page and Apple Weather mark.

### Instance Methods

func dailyStatistics&lt;each T>(for: CLLocation, forDaysIn: DateInterval, including: repeat DailyWeatherStatisticsQuery&lt;each T>) async throws -> (repeat DailyWeatherStatistics&lt;each T>)

Returns daily weather statistics for the requested location, for each day within the specified date interval.

func dailyStatistics&lt;each T>(for: CLLocation, including: repeat DailyWeatherStatisticsQuery&lt;each T>) async throws -> (repeat DailyWeatherStatistics&lt;each T>)

Returns daily weather statistics for the requested location, for each day between 30 days ago and 10 days from now.

func dailyStatistics&lt;each T>(for: CLLocation, startDay: Int, endDay: Int, including: repeat DailyWeatherStatisticsQuery&lt;each T>) async throws -> (repeat DailyWeatherStatistics&lt;each T>)

Returns daily weather statistics for the requested location, for each day from the start day to the end day, inclusively.

func dailySummary&lt;each T>(for: CLLocation, forDaysIn: DateInterval, including: repeat DailyWeatherSummaryQuery&lt;each T>) async throws -> (repeat DailyWeatherSummary&lt;each T>)

Returns day weather summaries for the requested location, for each day within the provided date interval.

func dailySummary&lt;each T>(for: CLLocation, including: repeat DailyWeatherSummaryQuery&lt;each T>) async throws -> (repeat DailyWeatherSummary&lt;each T>)

Returns day weather summaries for the requested location, for the past 30 days, including the present day.

func hourlyStatistics&lt;each T>(for: CLLocation, forHoursIn: DateInterval, including: repeat HourlyWeatherStatisticsQuery&lt;each T>) async throws -> (repeat HourlyWeatherStatistics&lt;each T>)

Returns hourly weather statistics for the requested location, for each hour within the specified date interval.

func hourlyStatistics&lt;each T>(for: CLLocation, including: repeat HourlyWeatherStatisticsQuery&lt;each T>) async throws -> (repeat HourlyWeatherStatistics&lt;each T>)

Returns hourly weather statistics for the requested location, for the 24 hours of the current day.

func hourlyStatistics&lt;each T>(for: CLLocation, startHour: Int, endHour: Int, including: repeat HourlyWeatherStatisticsQuery&lt;each T>) async throws -> (repeat HourlyWeatherStatistics&lt;each T>)

Returns hourly weather statistics for the requested location, for each hour from the start hour to the end hour, inclusively.

func monthlyStatistics&lt;each T>(for: CLLocation, forMonthsIn: DateInterval, including: repeat MonthlyWeatherStatisticsQuery&lt;each T>) async throws -> (repeat MonthlyWeatherStatistics&lt;each T>)

Returns monthly weather statistics for the requested location, for each month within the specified date interval.

func monthlyStatistics&lt;each T>(for: CLLocation, including: repeat MonthlyWeatherStatisticsQuery&lt;each T>) async throws -> (repeat MonthlyWeatherStatistics&lt;each T>)

Returns monthly weather statistics for the requested location, for all 12 months of the Gregorian calendar year.

func monthlyStatistics&lt;each T>(for: CLLocation, startMonth: Int, endMonth: Int, including: repeat MonthlyWeatherStatisticsQuery&lt;each T>) async throws -> (repeat MonthlyWeatherStatistics&lt;each T>)

Returns monthly weather statistics for the requested location, for each month from the start month to the end month, inclusively.

func weather&lt;T>(for: CLLocation, including: WeatherQuery&lt;T>) async throws -> T

Returns the weather forecast for the requested location.

func weather&lt;each T>(for: CLLocation, including: repeat WeatherQuery&lt;each T>) async throws -> (repeat each T)

Returns the weather forecast for the requested location.

## Relationships

### Conforms To

- Sendable

## See Also

### Fundamentals

Fetching weather forecasts with WeatherKit

Request and display weather data for destination airports in a flight-planning app.

struct Weather

A model representing the aggregate weather data the caller requests.

