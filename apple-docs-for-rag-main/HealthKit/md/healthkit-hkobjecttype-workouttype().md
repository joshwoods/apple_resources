

- HealthKit
- HKObjectType
-  workoutType() 

Type Method

# workoutType()

Returns the shared HKWorkoutType object.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 13.0+visionOS 1.0+watchOS 2.0+

``` source
class func workoutType() -> HKWorkoutType
```

## Return Value

The shared HKWorkoutType instance.

## Discussion

This method returns an instance of the HKWorkoutType concrete subclass. HealthKit uses workout types to create samples that store information about individual workouts. Use workout type instances to create workout objects that you can save in the HealthKit store. For more information, see HKWorkoutType.

In HealthKit, all workouts use the same workout type.

