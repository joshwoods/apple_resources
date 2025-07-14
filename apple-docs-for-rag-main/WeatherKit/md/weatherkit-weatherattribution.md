

- WeatherKit
-  WeatherAttribution 

Structure

# WeatherAttribution

A structure that defines the necessary information for attributing a weather data provider.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
struct WeatherAttribution
```

## Overview

Attribution is required for publishing software using WeatherKit.

## Topics

### Getting the properties

var combinedMarkDarkURL: URL

A URL for the combined “ Apple Weather” mark, in dark variant.

var combinedMarkLightURL: URL

A URL for the combined “ Apple Weather” mark, in light variant.

var legalPageURL: URL

A link to the legal attribution page that contains copyright information about the weather data sources.

var serviceName: String

The weather data provider name.

var squareMarkURL: URL

A URL for the square Apple Weather mark.

### Instance Properties

var legalAttributionText: String

This property returns text that should be made available to users for apps that cannot display the attributionURL contents in a Safari view. It contains language that outlines the weather data sources attribution and is a legal requirement of using WeatherKit.

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

struct WeatherMetadata

A structure that provides additional weather information.

enum WeatherSeverity

A description of the severity of the severe weather event.

