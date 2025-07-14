

- HealthKit
- HKHealthStore
-  biologicalSex() 

Instance Method

# biologicalSex()

Reads someone’s biological sex from the HealthKit store.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 13.0+visionOS 1.0+watchOS 2.0+

``` source
func biologicalSex() throws -> HKBiologicalSexObject
```

## Return Value

An object containing information about someone’s biological sex.

## Mentioned in 

About the HealthKit framework

## Discussion

For a list of possible values, see HKBiologicalSex.

If a person hasn’t set their biological sex or if they’ve denied permission to read the biological sex, this method returns an HKBiologicalSex.notSet value.

Handling Errors in Swift

In Swift, this method returns a nonoptional result and is marked with the `throws` keyword to indicate that it throws an error in cases of failure.

You call this method in a `try` expression and handle any errors in the `catch` clauses of a `do` statement, as described in Error Handling in The Swift Programming Language and About Imported Cocoa Error Parameters.

## Topics

### Possible Values

class HKBiologicalSexObject

This class acts as a wrapper for the HKBiologicalSex enumeration.

enum HKBiologicalSex

Constants indicating the user’s sex.

## See Also

### Reading characteristic data

func bloodType() throws -> HKBloodTypeObject

Reads the user’s blood type from the HealthKit store.

func dateOfBirth() throws -> Date

Reads the user’s date of birth from the HealthKit store as a date value.

Deprecated

func dateOfBirthComponents() throws -> DateComponents

Reads the user’s date of birth from the HealthKit store as date components.

func fitzpatrickSkinType() throws -> HKFitzpatrickSkinTypeObject

Reads the user’s Fitzpatrick Skin Type from the HealthKit store.

func wheelchairUse() throws -> HKWheelchairUseObject

Reads the user’s wheelchair use from the HealthKit store.

