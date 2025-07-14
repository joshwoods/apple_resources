

- Foundation
- Locale
-  availableNumberingSystems 

Instance Property

# availableNumberingSystems

An array containing all the valid numbering systems for the locale.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
var availableNumberingSystems: [Locale.NumberingSystem] { get }
```

## Discussion

The following snippet creates a locale for Arabic as used in United Arab Emirites. For this locale, there are two numbering systems available: `latn` (Latin digits) and `arab` (Arabic-Indic digits).

```
let uae = Locale(identifier: "ar-AE") // Arabic / U.A.E.
let numberingSystems = uae.availableNumberingSystems
print("\(numberingSystems.map{$0.identifier})") // ["latn","arab"]
```

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

struct NumberingSystem

A type that represents the numbering system used in a locale.

