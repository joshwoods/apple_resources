

- Foundation
- NSMeasurement
-  converting(to:) 

Instance Method

# converting(to:)

Returns a measurement created by converting the receiver to the specified unit.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+watchOS 3.0+

``` source
func converting(to unit: Unit) -> Measurement
```

## Parameters 

`unit`  

The unit to convert the measurement into.

## Return Value

A new measurement with a value calculated by converting into the new unit.

## Discussion

This method raises an invalidArgumentException if the receiver cannot be converted to unit.

## See Also

### Converting to Other Units

func canBeConverted(to: Unit) -> Bool

Indicates whether the measurement can be converted to the given unit.

