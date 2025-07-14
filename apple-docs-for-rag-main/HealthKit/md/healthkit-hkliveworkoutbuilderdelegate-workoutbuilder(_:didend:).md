

- HealthKit
- HKLiveWorkoutBuilderDelegate
-  workoutBuilder(\_:didEnd:) 

Instance Method

# workoutBuilder(\_:didEnd:)

Tells the delegate that the current workout activity has ended.

macOS 13.0+watchOS 9.0+

``` source
optional func workoutBuilder(
    _ workoutBuilder: HKLiveWorkoutBuilder,
    didEnd workoutActivity: HKWorkoutActivity
)
```

## Parameters 

`workoutBuilder`  

The workout builder that received the new activity.

`workoutActivity`  

The workout activity that just ended.

## See Also

### Tracking Live Data

func workoutBuilder(HKLiveWorkoutBuilder, didCollectDataOf: Set&lt;HKSampleType>)

Tells the delegate that new data has been added to the builder.

**Required**

func workoutBuilderDidCollectEvent(HKLiveWorkoutBuilder)

Tells the delegate that a new event has been added to the builder.

**Required**

func workoutBuilder(HKLiveWorkoutBuilder, didBegin: HKWorkoutActivity)

Tells the delegate that a new workout activity has started.

