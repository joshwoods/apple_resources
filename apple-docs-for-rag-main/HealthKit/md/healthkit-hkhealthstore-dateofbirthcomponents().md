

- HealthKit
- HKHealthStore
-  dateOfBirthComponents() 

Instance Method

# dateOfBirthComponents()

Reads the user’s date of birth from the HealthKit store as date components.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.0+macOS 13.0+visionOS 1.0+watchOS 3.0+

``` source
func dateOfBirthComponents() throws -> DateComponents
```

## Return Value

An NSDateComponents object representing the user’s birthdate in the Gregorian calendar, or `nil`.

## Discussion

If the user has not yet specified a birth date, or if the user has denied your app permission to read the birth date, this method returns `nil`.

## See Also

### Reading characteristic data

func biologicalSex() throws -> HKBiologicalSexObject

Reads someone’s biological sex from the HealthKit store.

func bloodType() throws -> HKBloodTypeObject

Reads the user’s blood type from the HealthKit store.

func dateOfBirth() throws -> Date

Reads the user’s date of birth from the HealthKit store as a date value.

Deprecated

func fitzpatrickSkinType() throws -> HKFitzpatrickSkinTypeObject

Reads the user’s Fitzpatrick Skin Type from the HealthKit store.

func wheelchairUse() throws -> HKWheelchairUseObject

Reads the user’s wheelchair use from the HealthKit store.

