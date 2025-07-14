

- HealthKit
- HKHealthStore
-  bloodType() 

Instance Method

# bloodType()

Reads the user’s blood type from the HealthKit store.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 13.0+visionOS 1.0+watchOS 2.0+

``` source
func bloodType() throws -> HKBloodTypeObject
```

## Return Value

A blood type object that contains information about the user’s blood type.

## Mentioned in 

About the HealthKit framework

## Discussion

If the user has not specified a blood type or if the user has denied your app permission to read the blood type, this method returns an HKBloodType.notSet value.

Handling Errors in Swift

In Swift, this method returns a nonoptional result and is marked with the `throws` keyword to indicate that it throws an error in cases of failure.

You call this method in a `try` expression and handle any errors in the `catch` clauses of a `do` statement, as described in Error Handling in The Swift Programming Language and `About Imported Cocoa Error Parameters`.

## Topics

### Possible Values

class HKBloodTypeObject

This class acts as a wrapper for the HKBloodType enumeration.

enum HKBloodType

Constants indicating the user’s blood type.

## See Also

### Reading characteristic data

func biologicalSex() throws -> HKBiologicalSexObject

Reads someone’s biological sex from the HealthKit store.

func dateOfBirth() throws -> Date

Reads the user’s date of birth from the HealthKit store as a date value.

Deprecated

func dateOfBirthComponents() throws -> DateComponents

Reads the user’s date of birth from the HealthKit store as date components.

func fitzpatrickSkinType() throws -> HKFitzpatrickSkinTypeObject

Reads the user’s Fitzpatrick Skin Type from the HealthKit store.

func wheelchairUse() throws -> HKWheelchairUseObject

Reads the user’s wheelchair use from the HealthKit store.

