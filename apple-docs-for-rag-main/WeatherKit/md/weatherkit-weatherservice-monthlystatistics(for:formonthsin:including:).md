

- WeatherKit
- WeatherService
-  monthlyStatistics(for:forMonthsIn:including:) 

Instance Method

# monthlyStatistics(for:forMonthsIn:including:)

Returns monthly weather statistics for the requested location, for each month within the specified date interval.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
final func monthlyStatistics(
    for location: CLLocation,
    forMonthsIn interval: DateInterval,
    including dataSets: repeat MonthlyWeatherStatisticsQuery
) async throws -> (repeat MonthlyWeatherStatistics) where repeat each T : Decodable, repeat each T : Encodable, repeat each T : Equatable, repeat each T : Sendable
```

## Parameters 

`location`  

The requested location.

`interval`  

The date interval for which to obtain monthly weather statistics. The end date of the interval will be capped at 1 year after the start date.

## Return Value

The requested monthly weather statistics.

## Discussion

Throws

Weather data error `WeatherError`

The statistics returned for each month are derived from weather data recorded over the past decades, to the present date. Each item returned represents statistics for a particular Gregorian Calendar month of the year.

This is a variadic API in which any combination of data sets can be requested and returned as a tuple. Here’s an example:

```
let (monthlyPrecipitationStatistics, monthlyTemperatureStatistics) = try await service.monthlyStatistics(for: newYork, forMonthsIn: interval, including: .precipitation, .temperature)
```

