

- WeatherKit
- WeatherService
-  weather(for:including:) 

Instance Method

# weather(for:including:)

Returns the weather forecast for the requested location.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
final func weather(
    for location: CLLocation,
    including dataSet: WeatherQuery
) async throws -> T
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
let current = try await service.weather(for: newYork, including: .current)
```

