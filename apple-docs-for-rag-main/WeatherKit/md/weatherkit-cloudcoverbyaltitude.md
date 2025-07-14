

- WeatherKit
-  CloudCoverByAltitude 

Structure

# CloudCoverByAltitude

Contains the percentage of sky covered by low, medium and high altitude cloud.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
struct CloudCoverByAltitude
```

## Topics

### Instance Properties

var high: Double

The percentage of the sky covered with high-altitude clouds. High-level Cloud Cover (HCC)corresponds to levels higher than 6300m above the model’s earth surface.

var low: Double

The percentage of the sky covered with low-altitude clouds. Low-level Cloud Cover (LCC) corresponds to levels between 0m and 1800m above the model’s earth surface.

var medium: Double

The percentage of the sky covered with mid-altitude clouds. Medium-level Cloud Cover (MCC) corresponds to levels between 1800m and 6300m above the model’s earth surface.

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

