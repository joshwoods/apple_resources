

- WeatherKit
-  WeatherAvailability 

Structure

# WeatherAvailability

A structure that indicates the availability of data at the requested location.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
struct WeatherAvailability
```

## Overview

`WeatherAvailability` represents the availability of data at the requested location. Weather alerts, or minute forecast data may be temporarily unavailable from the data provider, or unsupported in some regions. Other data sets are expected to be supported for all geographic locations, for example, current weather, and therefore are not included in `WeatherAvailability`.

## Topics

### Getting the properties

var alertAvailability: WeatherAvailability.AvailabilityKind

The weather alerts availability.

var minuteAvailability: WeatherAvailability.AvailabilityKind

The minute forecast availability.

enum AvailabilityKind

The availability kind.

### Default Implementations

Decodable Implementations

Encodable Implementations

Equatable Implementations

## Relationships

### Conforms To

- Copyable
- Decodable
- Encodable
- Equatable

## See Also

### Alerts and forecasts

struct WeatherAlert

A weather alert issued for the requested location by a governmental authority.

struct Forecast

A forecast collection for minute, hourly, and daily forecasts.

struct MinuteWeather

A structure that represents the next hour minute forecasts.

struct HourWeather

A structure that represents the weather conditions for the hour.

struct DayWeather

A structure that represents the weather conditions for the day.

