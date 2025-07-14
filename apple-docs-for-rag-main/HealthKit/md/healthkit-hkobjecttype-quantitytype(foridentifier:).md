

- HealthKit
- HKObjectType
-  quantityType(forIdentifier:) 

Type Method

# quantityType(forIdentifier:)

Returns the shared quantity type for the provided identifier.

iOS 8.0–18.4DeprecatediPadOS 8.0–18.4DeprecatedMac Catalyst 13.1+macOS 13.0+visionOS 1.0–2.4DeprecatedwatchOS 2.0–11.4Deprecated

``` source
class func quantityType(forIdentifier identifier: HKQuantityTypeIdentifier) -> HKQuantityType?
```

## Parameters 

`identifier`  

A quantity type identifier. For a list of valid identifiers, see HKQuantityTypeIdentifier.

## Return Value

The shared `HKQuantityType` instance based on the provided identifier.

## Mentioned in 

Saving data to HealthKit

## Discussion

This method returns an instance of the HKQuantityType concrete subclass. HealthKit uses quantity types to create samples that store a numerical value. Use quantity type instances to create quantity samples that you can save in the HealthKit store. For more information, see HKQuantitySample.

## See Also

### Creating quantity types

struct HKQuantityTypeIdentifier

The identifiers that create quantity type objects.

