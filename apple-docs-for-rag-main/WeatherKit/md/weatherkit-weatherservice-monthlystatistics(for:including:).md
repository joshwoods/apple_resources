

- WeatherKit
- WeatherService
-  monthlyStatistics(for:including:) 

Instance Method

# monthlyStatistics(for:including:)

Returns monthly weather statistics for the requested location, for all 12 months of the Gregorian calendar year.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
final func monthlyStatistics(
    for location: CLLocation,
    including dataSets: repeat MonthlyWeatherStatisticsQuery
) async throws -> (repeat MonthlyWeatherStatistics) where repeat each T : Decodable, repeat each T : Encodable, repeat each T : Equatable, repeat each T : Sendable
```

## Parameters 

`location`  

The requested location.

## Return Value

The requested monthly weather statistics

## Discussion

Throws

Weather data error `WeatherError`

The statistics returned for each month are derived from weather data recorded over the past decades, to the present date. Each item returned represents statistics for a particular Gregorian Calendar month of the year.

This is a variadic API in which any combination of data sets can be requested and returned as a tuple. Here’s an example:

```
let (monthlyPrecipitationStatistics, monthlyTemperatureStatistics) = try await service.monthlyStatistics(for: newYork, including: .precipitation, .temperature)
```

