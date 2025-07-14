

- HealthKit
- HKWorkoutSession
-  beginNewActivity(configuration:date:metadata:) 

Instance Method

# beginNewActivity(configuration:date:metadata:)

Begins a new workout activity in the workout session.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOSvisionOS 1.0+watchOS 9.0+

``` source
func beginNewActivity(
    configuration workoutConfiguration: HKWorkoutConfiguration,
    date: Date,
    metadata: [String : Any]?
)
```

## Parameters 

`workoutConfiguration`  

The configuration information for the activity. For HKWorkoutActivityType.swimBikeRun workouts, the activity’s configuration must use the HKWorkoutActivityType.swimming, HKWorkoutActivityType.cycling, or HKWorkoutActivityType.running activity types. For interval training, the activity’s configuration must use the same activity type as the containing workout.

`date`  

The activity’s start date and time.

`metadata`  

Metadata that provides additional information about the activity.

## Mentioned in 

Dividing a HealthKit workout into activities

## Discussion

This method asynchronously creates a new workout activity. HealthKit calls the session delegate’s workoutSession(_:didBeginActivityWith:date:) method after the activity begins. If the workout already has a current activity, HealthKit also ends that activity.

HealthKit may also set the data source’s typesToCollect value based on the new activity. If you’ve never modified the types that the data source collects (for example, by calling enableCollection(for:predicate:) or disableCollection(for:)), HealthKit automatically sets the typesToCollect property to a set of relevant data types based on the new actiity. However, if you’ve explicitly set the collected data types, HealthKit won’t modify them; therefore, you may need to update them for the new activity.

## See Also

### Managing workout activities

var currentActivity: HKWorkoutActivity

The current workout activity.

func endCurrentActivity(on: Date)

Ends the current workout activity.

