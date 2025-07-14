

- Foundation
- Locale
-  Locale.Currency 

Structure

# Locale.Currency

A type that represents the currency system used by a locale, like dollars or euros.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
struct Currency
```

## Topics

### Creating a currency instance

init(String)

Creates a currency instance from a BCP 47 identifier.

### Examining currency properties

var identifier: String

The currency’s identifier.

var isISOCurrency: Bool

A Boolean value that indicates whether the currency is in the list of ISO-defined currencies.

### Using common currencies

static var isoCurrencies: [Locale.Currency]

An array containing currencies defined by the currency codes in ISO-4217.

static let unknown: Locale.Currency

A representation of an “unknown” currency, for use with transactions that don’t involve any currency.

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

var measurementSystem: Locale.MeasurementSystem

The measurement system used by the locale, like metric or the US system.

struct MeasurementSystem

A type that represents the measurement system used by a locale, like metric or the US system.

var numberingSystem: Locale.NumberingSystem

The numbering system used by the locale.

var availableNumberingSystems: [Locale.NumberingSystem]

An array containing all the valid numbering systems for the locale.

struct NumberingSystem

A type that represents the numbering system used in a locale.

