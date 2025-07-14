

- WeatherKit
-  UVIndex 

Structure

# UVIndex

The expected intensity of ultraviolet radiation from the sun.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
struct UVIndex
```

## Topics

### Getting the UV index

var category: UVIndex.ExposureCategory

The UV Index exposure category.

var value: Int

The UV Index value.

enum ExposureCategory

An enumeration that indicates risk of harm from unprotected sun exposure.

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

### Characteristics

enum Precipitation

The form of precipitation.

enum PressureTrend

The atmospheric pressure change over time.

struct Wind

Contains wind data of speed, direction, and gust.

enum WeatherCondition

A description of the current weather condition.

