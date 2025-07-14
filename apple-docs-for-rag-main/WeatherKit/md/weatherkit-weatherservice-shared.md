

- WeatherKit
- WeatherService
-  shared 

Type Property

# shared

A single, shared weather service object.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
static let shared: WeatherService
```

## Discussion

Use this object to interface to weather services in your application. If you need to prioritize weather information, create separate instances with `init`.

## See Also

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

