

- HealthKit
- HKHealthStore
-  wheelchairUse() 

Instance Method

# wheelchairUse()

Reads the user’s wheelchair use from the HealthKit store.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.0+macOS 13.0+visionOS 1.0+watchOS 3.0+

``` source
func wheelchairUse() throws -> HKWheelchairUseObject
```

## Return Value

An object indicating whether the user uses a wheelchair.

## Discussion

If the user has not yet specified their wheelchair use, or if the user has denied your app permission to read the wheelchair use, this method returns HKWheelchairUse.notSet.

## Topics

### Possible Values

class HKWheelchairUseObject

This class acts as a wrapper for the wheelchair use enumeration.

enum HKWheelchairUse

Constants indicating the user’s wheelchair use.

## See Also

### Reading characteristic data

func biologicalSex() throws -> HKBiologicalSexObject

Reads someone’s biological sex from the HealthKit store.

func bloodType() throws -> HKBloodTypeObject

Reads the user’s blood type from the HealthKit store.

func dateOfBirth() throws -> Date

Reads the user’s date of birth from the HealthKit store as a date value.

Deprecated

func dateOfBirthComponents() throws -> DateComponents

Reads the user’s date of birth from the HealthKit store as date components.

func fitzpatrickSkinType() throws -> HKFitzpatrickSkinTypeObject

Reads the user’s Fitzpatrick Skin Type from the HealthKit store.

