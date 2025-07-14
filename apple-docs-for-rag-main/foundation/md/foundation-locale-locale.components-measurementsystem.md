

- Foundation
- Locale
- Locale.Components
-  measurementSystem 

Instance Property

# measurementSystem

The measurement system used by the locale, like metric or the US system.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
var measurementSystem: Locale.MeasurementSystem?
```

## Discussion

Set this property to override the locale’s default measurement system. To request the default measurement system used by the locale, use the Locale property `measurementSystem`.

This property corresponds to the `ms` key of the Unicode BCP 47 extension.

## See Also

### Specifiying measurement and counting components

var currency: Locale.Currency?

The currency used by the locale.

struct Currency

A type that represents the currency system used by a locale, like dollars or euros.

struct MeasurementSystem

A type that represents the measurement system used by a locale, like metric or the US system.

var numberingSystem: Locale.NumberingSystem?

The numbering system used by the locale.

struct NumberingSystem

A type that represents the numbering system used in a locale.

