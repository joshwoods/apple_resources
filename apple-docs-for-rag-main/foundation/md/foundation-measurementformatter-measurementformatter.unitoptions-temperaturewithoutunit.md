

- Foundation
- MeasurementFormatter
- MeasurementFormatter.UnitOptions
-  temperatureWithoutUnit 

Type Property

# temperatureWithoutUnit

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+watchOS 3.0+

``` source
static var temperatureWithoutUnit: MeasurementFormatter.UnitOptions { get }
```

## Discussion

Specifies that representations of a measurement with the `NSTemperatureUnit` unit omit the letter denoting the temperature scale. For example, a temperature measurement with value equal to 72 using the degreeFahrenheit() would be represented as `72°` rather than `72°F`.

## See Also

### Constants

static var providedUnit: MeasurementFormatter.UnitOptions

static var naturalScale: MeasurementFormatter.UnitOptions

static var providedUnit: MeasurementFormatter.UnitOptions

static var naturalScale: MeasurementFormatter.UnitOptions

