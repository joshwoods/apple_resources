

- WeatherKit
-  DailyWeatherStatisticsQuery 

Structure

# DailyWeatherStatisticsQuery

A structure that encapsulates a generic daily weather statistics dataset request.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
struct DailyWeatherStatisticsQuery where T : Decodable, T : Encodable, T : Equatable
```

## Overview

Use the properties of this structure to create a daily weather statistics query. You can combine multiple queries into a single `WeatherService` request.

Here’s how to get daily weather statistics for New York City:

```
```

## Topics

### Type Properties

static var precipitation: DailyWeatherStatisticsQuery&lt;DayPrecipitationStatistics>

The daily precipitation statistics query.

static var temperature: DailyWeatherStatisticsQuery&lt;DayTemperatureStatistics>

The daily temperature statistics query.

