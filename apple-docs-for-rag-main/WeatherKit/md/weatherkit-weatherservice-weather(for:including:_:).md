

- WeatherKit
- WeatherService
-  weather(for:including:\_:) 

Instance Method

# weather(for:including:\_:)

Returns the weather forecast for the requested location.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
final func weather(
    for location: CLLocation,
    including dataSet1: WeatherQuery,
    _ dataSet2: WeatherQuery
) async throws -> (T1, T2)
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
let (current, minute) = try await service.weather(for: newYork, including: .current, .minute)
```

## See Also

### Obtaining forecasts

func weather(for: CLLocation) async throws -> Weather

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

