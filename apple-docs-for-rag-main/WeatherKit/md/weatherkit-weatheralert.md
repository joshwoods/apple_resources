

- WeatherKit
-  WeatherAlert 

Structure

# WeatherAlert

A weather alert issued for the requested location by a governmental authority.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
struct WeatherAlert
```

## Overview

Weather alerts often contains severe weather information; however, not all alerts are severe. Alerts may or may not contain localized descriptions, depending on what is available from the source. Due to data source restrictions, information contained is served raw.

## Topics

### Getting the properties

var metadata: WeatherMetadata

Descriptive information about the weather alert data.

var region: String?

The name of the affected area.

var severity: WeatherSeverity

The severity of the weather alert.

var summary: String

The summary of the event type.

### Providing attribution

var detailsURL: URL

The site for more details about the weather alert.

var source: String

The name of the source issuing the weather alert.

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

struct WeatherAvailability

A structure that indicates the availability of data at the requested location.

struct Forecast

A forecast collection for minute, hourly, and daily forecasts.

struct MinuteWeather

A structure that represents the next hour minute forecasts.

struct HourWeather

A structure that represents the weather conditions for the hour.

struct DayWeather

A structure that represents the weather conditions for the day.

