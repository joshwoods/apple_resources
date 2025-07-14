

- WeatherKit
-  HourlyWeatherStatisticsQuery 

Structure

# HourlyWeatherStatisticsQuery

A structure that encapsulates a generic hourly weather statistics dataset request.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
struct HourlyWeatherStatisticsQuery where T : Decodable, T : Encodable, T : Equatable
```

## Overview

Use the properties of this structure to create an hourly weather statistics query. You can combine multiple queries into a single `WeatherService` request.

Here’s how to get hourly weather statistics for New York City:

```
let (hourlyTemperatureStatistics) = try await service.hourlyStatistics(for: newYork, spanning: timeInterval, including: .temperature)
```

## Topics

### Type Properties

static var temperature: HourlyWeatherStatisticsQuery&lt;HourTemperatureStatistics>

The hourly temperature statistics query.

