

- Foundation
- Locale
-  measurementSystem 

Instance Property

# measurementSystem

The measurement system used by the locale, like metric or the US system.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
var measurementSystem: Locale.MeasurementSystem { get }
```

## Discussion

When called on the special Locale instances current or autoupdatingCurrent, if the user overrode the default measurement system, this property provides the user’s preference.

This property corresponds to the `ms` key of the Unicode BCP 47 extension.

For locale instances created with the `ms` specifier (such as `en-US@ms=metric`), or with a custom Locale.Components, this property represents the custom measurement system. Otherwise, it represents the locale’s default measurement system.

## See Also

### Getting measurement and counting components

var currency: Locale.Currency?

The currency used by the locale.

struct Currency

A type that represents the currency system used by a locale, like dollars or euros.

struct MeasurementSystem

A type that represents the measurement system used by a locale, like metric or the US system.

var numberingSystem: Locale.NumberingSystem

The numbering system used by the locale.

var availableNumberingSystems: [Locale.NumberingSystem]

An array containing all the valid numbering systems for the locale.

struct NumberingSystem

A type that represents the numbering system used in a locale.

