

- Foundation
- MeasurementFormatter
-  string(from:) 

Instance Method

# string(from:)

Creates and returns a localized string representation of the provided unit of measure.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+watchOS 3.0+

``` source
func string(from unit: Unit) -> String
```

## Parameters 

`unit`  

The unit of measure to be represented.

## Return Value

A user-readable string that represents the unit of measure. If the unit cannot be localized, the unit’s symbol value is used.

## See Also

### Converting Measurements

func string(from: Measurement&lt;Unit>) -> String

Creates and returns a localized string representation of the provided measurement.

