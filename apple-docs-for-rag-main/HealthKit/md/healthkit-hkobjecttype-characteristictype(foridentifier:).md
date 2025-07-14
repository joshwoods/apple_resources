

- HealthKit
- HKObjectType
-  characteristicType(forIdentifier:) 

Type Method

# characteristicType(forIdentifier:)

Returns the shared characteristic type for the provided identifier.

iOS 8.0–18.4DeprecatediPadOS 8.0–18.4DeprecatedMac Catalyst 13.1+macOS 13.0+visionOS 1.0–2.4DeprecatedwatchOS 2.0–11.4Deprecated

``` source
class func characteristicType(forIdentifier identifier: HKCharacteristicTypeIdentifier) -> HKCharacteristicType?
```

## Parameters 

`identifier`  

A characteristic type identifier. For a list of valid identifiers, see HKCharacteristicTypeIdentifier.

## Return Value

The shared `HKCharacteristicType` instance based on the provided identifier.

## Discussion

This method returns an instance of the HKCharacteristicType concrete subclass. Characteristic types represent data that doesn’t typically change over time. Unlike the other object types, characteristic types cannot be used to create new HealthKit objects. Instead, users must enter and edit their characteristic data using the Health app. Characteristic types are used only when asking for permission to read data from the HealthKit store.

## See Also

### Creating characteristic types

struct HKCharacteristicTypeIdentifier

The identifiers that create characteristic type objects.

