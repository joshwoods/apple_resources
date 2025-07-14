

- WeatherKit
- WeatherService
-  init() 

Initializer

# init()

Creates a weather service object.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
convenience init()
```

## Discussion

Use this method to create different `WeatherService` instances, for example, to separate out high-priority and low-priority requests for performance. If you only need one instance of `WeatherService`, use `shared`.

