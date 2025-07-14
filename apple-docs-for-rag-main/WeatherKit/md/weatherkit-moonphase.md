

- WeatherKit
-  MoonPhase 

Enumeration

# MoonPhase

An enumeration that specifies the moon phase kind.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
@frozen
enum MoonPhase
```

## Overview

Waxing and waning provide information about direction. Crescent and gibbous describe shape.

## Topics

### Creating the object

init?(rawValue: String)

Creates a new instance with the specified raw value.

### Getting the moon phase

case firstQuarter

The disk is half lit.

case full

The disk is fully lit where the moon is visible.

case lastQuarter

The disk is half lit.

case new

The disk is unlit where the moon is not visible.

case waningCrescent

The disk is partially lit as the moon is waning.

case waningGibbous

The disk is half lit as the moon is waning.

case waxingCrescent

The disk is partially lit as the moon is waxing.

case waxingGibbous

The disk is half lit as the moon is waxing.

### Describing the moon phase

var accessibilityDescription: String

A localized accessibility description describing the moon phase.

var description: String

A localized string describing the moon phase.

var symbolName: String

The SF Symbol icon that represents the moon phase.

### Instance Properties

var rawValue: String

The corresponding value of the raw type.

### Type Aliases

typealias AllCases

A type that can represent a collection of all values of this type.

typealias RawValue

The raw type that can be used to represent all values of the conforming type.

### Type Properties

static var allCases: [MoonPhase]

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

### Celestial information

struct SunEvents

An enumeration that represents dates of solar events, including sunrise, sunset, dawn, and dusk.

struct MoonEvents

A structure that represents lunar events.

