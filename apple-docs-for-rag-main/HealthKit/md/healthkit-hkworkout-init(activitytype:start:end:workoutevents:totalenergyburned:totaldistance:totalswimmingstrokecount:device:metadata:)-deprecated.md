

- HealthKit
- HKWorkout
-  init(activityType:start:end:workoutEvents:totalEnergyBurned:totalDistance:totalSwimmingStrokeCount:device:metadata:) Deprecated

Initializer

# init(activityType:start:end:workoutEvents:totalEnergyBurned:totalDistance:totalSwimmingStrokeCount:device:metadata:)

Instantiates a workout using a variety of data, including the number of strokes while swimming.

iOS 10.0–17.0DeprecatediPadOS 10.0–17.0DeprecatedMac Catalyst 13.0–16.0DeprecatedmacOS 13.0–14.0DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 3.0–10.0Deprecated

``` source
convenience init(
    activityType workoutActivityType: HKWorkoutActivityType,
    start startDate: Date,
    end endDate: Date,
    workoutEvents: [HKWorkoutEvent]?,
    totalEnergyBurned: HKQuantity?,
    totalDistance: HKQuantity?,
    totalSwimmingStrokeCount: HKQuantity?,
    device: HKDevice?,
    metadata: [String : Any]?
)
```

Deprecated

Use HKWorkoutBuilder

## Parameters 

`workoutActivityType`  

The type of activity performed during the workout. For the complete list of activity types, see HKWorkoutActivityType.

`startDate`  

The date and time when the activity started.

`endDate`  

The date and time when the activity ended. This date must be equal to or later than the start date.

`workoutEvents`  

An array of workout event objects. This array specifies when the user has paused and resumed the workout activity. This method calculates the workout’s duration based on the total amount of active time between the provided start and end dates.

`totalEnergyBurned`  

A quantity using energy units, or `nil`. This property sets the workout’s totalEnergyBurned property. It represents the total active energy burned during the workout.

`totalDistance`  

A quantity using length units, or `nil`. This property sets the workout’s totalDistance property.

`totalSwimmingStrokeCount`  

A quantity unit using count units or `nil`. This property sets the workout’s totalSwimmingStrokeCount property.

`device`  

The device that generated the data for this sample.

`metadata`  

The metadata dictionary contains extra information describing this workout. The dictionary’s keys are all NSString objects . The values may be NSString, NSNumber, or NSDate objects. For a complete list of predefined metadata keys, see Metadata Keys.

Using predefined keys helps facilitate sharing data between apps; however, you are also encouraged to create your own, custom keys as needed to extend the HealthKit quantity sample’s capabilities.

## Return Value

A workout object with the specified duration, total energy burned, total distance, total stroke count, device, metadata, and workout events.

## Discussion

This method calculates the workout’s duration based on the amount of time it spends in an active state. A workout starts in an active state. A pause event switches it to an inactive state, and a resume event switches it back to an active state. For more information on workout events, see HKWorkoutEvent.

If the total energy burned or total distance are non-zero values, create a set of corresponding samples that add up to the calculated totals. Associate these samples with the workout by calling the health store’s add(_:to:completion:) method.

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

convenience init(activityType: HKWorkoutActivityType, start: Date, end: Date)

Instantiates a new workout.

Deprecated

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

