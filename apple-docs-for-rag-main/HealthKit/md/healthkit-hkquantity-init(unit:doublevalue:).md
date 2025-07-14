

- HealthKit
- HKQuantity
-  init(unit:doubleValue:) 

Initializer

# init(unit:doubleValue:)

Instantiates and returns a new quantity object.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 13.0+visionOS 1.0+watchOS 2.0+

``` source
convenience init(
    unit: HKUnit,
    doubleValue value: Double
)
```

## Parameters 

`unit`  

The units for the given value. This defines the set of compatible units. For example, if you create a quantity with a meter unit, it is compatible with any other length units.

`value`  

The value of this quantity, measured using the unit parameter.

## Return Value

A newly instantiated quantity instance.

## Discussion

HealthKit uses quantity objects to store data for quantity samples. For more information on using quantity objects, see HKQuantitySample.

