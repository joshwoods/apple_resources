

- WeatherKit
- WeatherService
-  weather(for:including:) 

Instance Method

# weather(for:including:)

Returns the weather forecast for the requested location.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
final func weather(
    for location: CLLocation,
    including dataSet: repeat WeatherQuery
) async throws -> (repeat each T)
```

## Parameters 

`location`  

The requested location.

## Return Value

The requested weather data set.

## Discussion

Throws

Weather data error `WeatherError`

This is a variadic API in which any combination of data sets can be requested and returned as a tuple. Here’s an example:

```
`let (current, minute, hourly, daily, alerts) = try await service.weather(for: newYork, including: .current, .minute, .hourly, .daily, .alerts)`
```

