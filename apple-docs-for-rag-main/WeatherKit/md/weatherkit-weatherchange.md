

- WeatherKit
-  WeatherChange 

Structure

# WeatherChange

A structure that informs how certain measurable weather aspects are expected to change relative to before.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
struct WeatherChange
```

## Topics

### Instance Properties

var date: Date

The date at which this change record becomes effective.

var dayPrecipitationAmount: WeatherChange.Direction

How the forecasted precipitation amount for this day, during daylight hours, compares to that of before.

var highTemperature: WeatherChange.Direction

How the high temperature for this day compares to that of before.

var lowTemperature: WeatherChange.Direction

How the low temperature for this day compares to that of before.

var nightPrecipitationAmount: WeatherChange.Direction

How the forecasted precipitation amount, during the night of this day, compares to that of before.

### Enumerations

enum Direction

An enum that specifies the direction in which a measurable aspect of the weather is expected to change.

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

