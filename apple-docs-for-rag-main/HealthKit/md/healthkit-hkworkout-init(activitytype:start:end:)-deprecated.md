

- HealthKit
- HKWorkout
-  init(activityType:start:end:) Deprecated

Initializer

# init(activityType:start:end:)

Instantiates a new workout.

iOS 8.0–17.0DeprecatediPadOS 8.0–17.0DeprecatedMac Catalyst 13.0–16.0DeprecatedmacOS 13.0–14.0DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 2.0–10.0Deprecated

``` source
convenience init(
    activityType workoutActivityType: HKWorkoutActivityType,
    start startDate: Date,
    end endDate: Date
)
```

Deprecated

Use HKWorkoutBuilder

## Parameters 

`workoutActivityType`  

The type of activity being performed during the workout. For a list of possible activity types, see HKWorkoutActivityType.

`startDate`  

The date and time when the activity started.

`endDate`  

The date and time when the activity ended. This date must be equal to or later than the start date.

## Return Value

A workout activity.

## Discussion

The workout’s duration is calculated from its start and end times. The workout’s total distance, total energy burned, workout events, device, and metadata are all set to `nil`.

- Swift
- Objective-C

```
let basketball = HKWorkout(activityType:HKWorkoutActivityType.Basketball,
                           startDate: start, endDate: end)

healthStore.saveObject(basketball) { (success, error) -> Void in
    guard success else {
        // Perform proper error handling here...
        fatalError("*** An error occurred while saving this " +
            "workout: \(error?.localizedDescription)")
    }
}
```

```
HKWorkout *basketball =
[HKWorkout workoutWithActivityType:HKWorkoutActivityTypeBasketball
                         startDate:start
                           endDate:end];

[self.healthStore
 saveObject:basketball
 withCompletion:^(BOOL success, NSError *error) {

     if (!success) {
         // Perform proper error handling here...
         NSLog(@"*** An error occurred while saving this "
               @"workout: %@ ***", error.localizedDescription);
     }

 }];
```

## See Also

### Related Documentation

var workoutActivityType: HKWorkoutActivityType

The type of activity performed during the workout.

var totalDistance: HKQuantity?

The total distance traveled during the workout.

Deprecated

var duration: TimeInterval

The workout’s duration.

var metadata: [String : Any]?

The metadata for this HealthKit object.

var totalEnergyBurned: HKQuantity?

The total active energy burned during the workout.

Deprecated

var workoutEvents: [HKWorkoutEvent]?

An array of workout event objects.

### Creating workouts

convenience init(activityType: HKWorkoutActivityType, start: Date, end: Date, duration: TimeInterval, totalEnergyBurned: HKQuantity?, totalDistance: HKQuantity?, metadata: [String : Any]?)

Instantiates a new workout that includes the energy burned, distance, and metadata for the workout.

Deprecated

convenience init(activityType: HKWorkoutActivityType, start: Date, end: Date, workoutEvents: [HKWorkoutEvent]?, totalEnergyBurned: HKQuantity?, totalDistance: HKQuantity?, metadata: [String : Any]?)

Instantiates a new workout whose duration is calculated based on the start and end dates and the provided workout events.

Deprecated

convenience init(activityType: HKWorkoutActivityType, start: Date, end: Date, duration: TimeInterval, totalEnergyBurned: HKQuantity?, totalDistance: HKQuantity?, device: HKDevice?, metadata: [String : Any]?)

Instantiates a new workout activity that includes the device that produced the sample data.

Deprecated

convenience init(activityType: HKWorkoutActivityType, start: Date, end: Date, workoutEvents: [HKWorkoutEvent]?, totalEnergyBurned: HKQuantity?, totalDistance: HKQuantity?, device: HKDevice?, metadata: [String : Any]?)

Instantiates a workout that includes both workout events and the device that produced the sample data.

Deprecated

convenience init(activityType: HKWorkoutActivityType, start: Date, end: Date, workoutEvents: [HKWorkoutEvent]?, totalEnergyBurned: HKQuantity?, totalDistance: HKQuantity?, totalFlightsClimbed: HKQuantity?, device: HKDevice?, metadata: [String : Any]?)

Instantiates a workout using a variety of data, including the number of flights of stairs climbed.

Deprecated

convenience init(activityType: HKWorkoutActivityType, start: Date, end: Date, workoutEvents: [HKWorkoutEvent]?, totalEnergyBurned: HKQuantity?, totalDistance: HKQuantity?, totalSwimmingStrokeCount: HKQuantity?, device: HKDevice?, metadata: [String : Any]?)

Instantiates a workout using a variety of data, including the number of strokes while swimming.

Deprecated

