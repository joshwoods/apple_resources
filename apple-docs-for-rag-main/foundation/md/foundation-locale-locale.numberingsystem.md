

- Foundation
- Locale
-  Locale.NumberingSystem 

Structure

# Locale.NumberingSystem

A type that represents the numbering system used in a locale.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
struct NumberingSystem
```

## Topics

### Creating a numbering system instance

init(String)

Creates a numbering system instance from a BCP 47 identifier.

### Examining numbering system properties

var identifier: String

The numbering system’s BCP 47 identifier.

### Type Properties

static var availableNumberingSystems: [Locale.NumberingSystem]

## Relationships

### Conforms To

- Copyable
- CustomDebugStringConvertible
- Decodable
- Encodable
- Equatable
- ExpressibleByExtendedGraphemeClusterLiteral
- ExpressibleByStringLiteral
- ExpressibleByUnicodeScalarLiteral
- Hashable
- Sendable

## See Also

### Getting measurement and counting components

var currency: Locale.Currency?

The currency used by the locale.

struct Currency

A type that represents the currency system used by a locale, like dollars or euros.

var measurementSystem: Locale.MeasurementSystem

The measurement system used by the locale, like metric or the US system.

struct MeasurementSystem

A type that represents the measurement system used by a locale, like metric or the US system.

var numberingSystem: Locale.NumberingSystem

The numbering system used by the locale.

var availableNumberingSystems: [Locale.NumberingSystem]

An array containing all the valid numbering systems for the locale.

