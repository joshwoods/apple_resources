

- WeatherKit
-  WeatherQuery 

Structure

# WeatherQuery

A structure that encapsulates a generic weather dataset request.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
struct WeatherQuery
```

## Overview

Use the properties of this structure to create a weather query. You can combine multiple weather queries into a single WeatherService request.

Here’s how to get the weather for New York City:

```
let (hourly, daily, alerts) = try await service.weather(for: newYork, including: .hourly, .daily, .alerts)
```

## Topics

### Creating queries

static var alerts: WeatherQuery&lt;[WeatherAlert]?>

The weather alerts query.

static var availability: WeatherQuery&lt;WeatherAvailability>

The availability query.

static var current: WeatherQuery&lt;CurrentWeather>

The current weather query.

static var daily: WeatherQuery&lt;Forecast&lt;DayWeather>>

The daily forecast query. This returns 10 contiguous days, beginning with the current day.

static var hourly: WeatherQuery&lt;Forecast&lt;HourWeather>>

The hourly forecast query. This returns 25 contiguous hours, beginning with the current hour.

static var minute: WeatherQuery&lt;Forecast&lt;MinuteWeather>?>

The minute forecast query.

static func daily(startDate: Date, endDate: Date) -> WeatherQuery&lt;T>

Returns weather for an arbitrary range of days, with the following caveats:

static func hourly(startDate: Date, endDate: Date) -> WeatherQuery&lt;T>

The hourly forecast query that takes a start date and end date for the request, with the following caveats:

### Type Properties

static var changes: WeatherQuery&lt;WeatherChanges?>

The weather changes query.

static var historicalComparisons: WeatherQuery&lt;HistoricalComparisons?>

The weather historical comparison query.

## See Also

### Requests

struct CurrentWeather

A structure that describes the current conditions observed at a location.

struct WeatherAttribution

A structure that defines the necessary information for attributing a weather data provider.

struct WeatherMetadata

A structure that provides additional weather information.

enum WeatherSeverity

A description of the severity of the severe weather event.

