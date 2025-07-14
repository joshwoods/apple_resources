

- HealthKit
- HKObjectType
-  correlationType(forIdentifier:) 

Type Method

# correlationType(forIdentifier:)

Returns the shared correlation type for the provided identifier.

iOS 8.0–18.4DeprecatediPadOS 8.0–18.4DeprecatedMac Catalyst 13.1+macOS 13.0+visionOS 1.0–2.4DeprecatedwatchOS 2.0–11.4Deprecated

``` source
class func correlationType(forIdentifier identifier: HKCorrelationTypeIdentifier) -> HKCorrelationType?
```

## Parameters 

`identifier`  

A correlation type identifier. For a list of valid identifiers, see HKCorrelationTypeIdentifier.

## Return Value

The shared HKCorrelationType instance based on the provided identifier.

## Discussion

This method returns an instance of the HKCorrelationType concrete subclass. HealthKit uses correlation types to create complex data objects that contain multiple values. Use correlation type instances to create correlation objects that you can save in the HealthKit store. For more information, see HKCorrelation.

## See Also

### Creating correlation types

struct HKCorrelationTypeIdentifier

The identifiers that create correlation type objects.

