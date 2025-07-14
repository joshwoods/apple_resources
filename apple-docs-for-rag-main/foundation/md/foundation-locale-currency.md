

- Foundation
- Locale
-  currency 

Instance Property

# currency

The currency used by the locale.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
var currency: Locale.Currency? { get }
```

## Discussion

This property corresponds to the `cu` key of the Unicode BCP 47 extension.

For locale instances created with the `cu` specifier (such as `en-US@cu=cad`), or with a custom Locale.Components, this property represents the custom currency. Otherwise, it represents the locale’s default currency.

## See Also

### Getting measurement and counting components

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

struct NumberingSystem

A type that represents the numbering system used in a locale.

