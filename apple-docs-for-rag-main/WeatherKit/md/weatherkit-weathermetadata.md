

- WeatherKit
-  WeatherMetadata 

Structure

# WeatherMetadata

A structure that provides additional weather information.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
struct WeatherMetadata
```

## Overview

Metadata information includes the location, date of the request, the date the data will expire, and required provider attribution.

## Topics

### Getting the properties

var date: Date

The time of the weather data request.

var expirationDate: Date

The time the weather data expires.

var location: CLLocation

The location of the request.

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

### Requests

struct WeatherQuery

A structure that encapsulates a generic weather dataset request.

struct CurrentWeather

A structure that describes the current conditions observed at a location.

struct WeatherAttribution

A structure that defines the necessary information for attributing a weather data provider.

enum WeatherSeverity

A description of the severity of the severe weather event.

