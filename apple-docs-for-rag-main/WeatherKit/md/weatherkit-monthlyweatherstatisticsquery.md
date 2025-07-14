

- WeatherKit
-  MonthlyWeatherStatisticsQuery 

Structure

# MonthlyWeatherStatisticsQuery

A structure that encapsulates a generic monthly weather statistics dataset request.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
struct MonthlyWeatherStatisticsQuery where T : Decodable, T : Encodable, T : Equatable
```

## Overview

Use the properties of this structure to create a monthly weather statistics query. You can combine multiple queries into a single `WeatherService` request.

Here’s how to get monthly weather statistics for New York City:

```
let (monthlyPrecipitationStatistics, monthlyTemperatureStatistics) = try await service.monthlyStatistics(for: newYork, spanning: interval, including: .precipitation, .temperature)
```

## Topics

### Type Properties

static var precipitation: MonthlyWeatherStatisticsQuery&lt;MonthPrecipitationStatistics>

The monthly precipitation statistics query.

static var temperature: MonthlyWeatherStatisticsQuery&lt;MonthTemperatureStatistics>

The monthly temperature statistics query.

