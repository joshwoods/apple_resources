

- HealthKit
- HKLiveWorkoutBuilderDelegate
-  workoutBuilder(\_:didBegin:) 

Instance Method

# workoutBuilder(\_:didBegin:)

Tells the delegate that a new workout activity has started.

macOS 13.0+watchOS 9.0+

``` source
optional func workoutBuilder(
    _ workoutBuilder: HKLiveWorkoutBuilder,
    didBegin workoutActivity: HKWorkoutActivity
)
```

## Parameters 

`workoutBuilder`  

The workout builder that received the new activity.

`workoutActivity`  

A new workout activity, currently in progress.

## See Also

### Tracking Live Data

func workoutBuilder(HKLiveWorkoutBuilder, didCollectDataOf: Set&lt;HKSampleType>)

Tells the delegate that new data has been added to the builder.

**Required**

func workoutBuilderDidCollectEvent(HKLiveWorkoutBuilder)

Tells the delegate that a new event has been added to the builder.

**Required**

func workoutBuilder(HKLiveWorkoutBuilder, didEnd: HKWorkoutActivity)

Tells the delegate that the current workout activity has ended.

