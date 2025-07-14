

- HealthKit
- HKHealthStore
-  dateOfBirth() Deprecated

Instance Method

# dateOfBirth()

Reads the user’s date of birth from the HealthKit store as a date value.

iOS 8.0–10.0DeprecatediPadOS 8.0–10.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 13.0+visionOS 1.0–1.0DeprecatedwatchOS 2.0–3.0Deprecated

``` source
func dateOfBirth() throws -> Date
```

Deprecated

Use dateOfBirthComponents() instead.

## Return Value

An NSDate object representing the user’s birthdate, or `nil`.

## Mentioned in 

About the HealthKit framework

## Discussion

If the user has not yet specified a birth date, or if the user has denied your app permission to read the birth date, this method returns `nil`.

Handling Errors in Swift

In Swift, this method returns a nonoptional result and is marked with the `throws` keyword to indicate that it throws an error in cases of failure.

You call this method in a `try` expression and handle any errors in the `catch` clauses of a `do` statement, as described in Error Handling in The Swift Programming Language and `About Imported Cocoa Error Parameters`.

## See Also

### Reading characteristic data

func biologicalSex() throws -> HKBiologicalSexObject

Reads someone’s biological sex from the HealthKit store.

func bloodType() throws -> HKBloodTypeObject

Reads the user’s blood type from the HealthKit store.

func dateOfBirthComponents() throws -> DateComponents

Reads the user’s date of birth from the HealthKit store as date components.

func fitzpatrickSkinType() throws -> HKFitzpatrickSkinTypeObject

Reads the user’s Fitzpatrick Skin Type from the HealthKit store.

func wheelchairUse() throws -> HKWheelchairUseObject

Reads the user’s wheelchair use from the HealthKit store.

