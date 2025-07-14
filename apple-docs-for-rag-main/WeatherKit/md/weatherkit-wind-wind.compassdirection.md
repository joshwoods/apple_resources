

- WeatherKit
- Wind
-  Wind.CompassDirection 

Enumeration

# Wind.CompassDirection

A compass composed of cardinal and intercardinal directions.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
@frozen
enum CompassDirection
```

## Overview

This enumeration represents true headings.

## Topics

### Creating the object

init?(rawValue: String)

Creates a new instance with the specified raw value.

### Describing the compass direction

var abbreviation: String

A localized short abbreviation of the wind compass direction.

var accessibilityDescription: String

A localized accessibility description describing the compass direction.

var description: String

A localized string describing the compass direction.

### Enumeration Cases

case east

case eastNortheast

case eastSoutheast

case north

case northNortheast

case northNorthwest

case northeast

case northwest

case south

case southSoutheast

case southSouthwest

case southeast

case southwest

case west

case westNorthwest

case westSouthwest

### Instance Properties

var rawValue: String

The corresponding value of the raw type.

### Type Aliases

typealias AllCases

A type that can represent a collection of all values of this type.

typealias RawValue

The raw type that can be used to represent all values of the conforming type.

### Type Properties

static var allCases: [Wind.CompassDirection]

A collection of all values of this type.

### Default Implementations

Equatable Implementations

RawRepresentable Implementations

## Relationships

### Conforms To

- BitwiseCopyable
- CaseIterable
- Copyable
- CustomStringConvertible
- Decodable
- Encodable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Getting the properties

var compassDirection: Wind.CompassDirection

The general indicator of wind direction.

var direction: Measurement&lt;UnitAngle>

The direction the wind is coming from in degrees.

var gust: Measurement&lt;UnitSpeed>?

A sudden increase in wind speed due to friction, wind shear, or by heating.

var speed: Measurement&lt;UnitSpeed>

Sustained wind speed.

