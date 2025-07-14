

- HealthKit
- HKObjectType
-  categoryType(forIdentifier:) 

Type Method

# categoryType(forIdentifier:)

Returns the shared category type for the provided identifier.

iOS 8.0–18.4DeprecatediPadOS 8.0–18.4DeprecatedMac Catalyst 13.1+macOS 13.0+visionOS 1.0–2.4DeprecatedwatchOS 2.0–11.4Deprecated

``` source
class func categoryType(forIdentifier identifier: HKCategoryTypeIdentifier) -> HKCategoryType?
```

## Parameters 

`identifier`  

A category type identifier. For a list of valid identifiers, see HKCategoryTypeIdentifier.

## Return Value

The shared `HKCategoryType` instance based on the provided identifier.

## Discussion

This method returns an instance of the HKCategoryType concrete subclass. HealthKit uses category types to represent data that can be categorized into an enumeration of values. Use category type instances to create category samples that you can then save in the HealthKit store. For more information, see HKCategorySample.

## See Also

### Creating category types

struct HKCategoryTypeIdentifier

Identifiers for creating category types.

