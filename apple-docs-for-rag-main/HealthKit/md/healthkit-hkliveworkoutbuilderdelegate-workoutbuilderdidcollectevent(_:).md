

- HealthKit
- HKLiveWorkoutBuilderDelegate
-  workoutBuilderDidCollectEvent(\_:) 

Instance Method

# workoutBuilderDidCollectEvent(\_:)

Tells the delegate that a new event has been added to the builder.

macOSwatchOS 5.0+

``` source
func workoutBuilderDidCollectEvent(_ workoutBuilder: HKLiveWorkoutBuilder)
```

**Required**

## Mentioned in 

Running workout sessions

## See Also

### Tracking Live Data

func workoutBuilder(HKLiveWorkoutBuilder, didCollectDataOf: Set&lt;HKSampleType>)

Tells the delegate that new data has been added to the builder.

**Required**

func workoutBuilder(HKLiveWorkoutBuilder, didBegin: HKWorkoutActivity)

Tells the delegate that a new workout activity has started.

func workoutBuilder(HKLiveWorkoutBuilder, didEnd: HKWorkoutActivity)

Tells the delegate that the current workout activity has ended.

