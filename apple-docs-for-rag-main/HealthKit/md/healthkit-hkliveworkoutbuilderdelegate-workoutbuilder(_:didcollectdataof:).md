

- HealthKit
- HKLiveWorkoutBuilderDelegate
-  workoutBuilder(\_:didCollectDataOf:) 

Instance Method

# workoutBuilder(\_:didCollectDataOf:)

Tells the delegate that new data has been added to the builder.

macOS 13.0+watchOS 5.0+

``` source
func workoutBuilder(
    _ workoutBuilder: HKLiveWorkoutBuilder,
    didCollectDataOf collectedTypes: Set
)
```

**Required**

## Mentioned in 

Running workout sessions

## See Also

### Tracking Live Data

func workoutBuilderDidCollectEvent(HKLiveWorkoutBuilder)

Tells the delegate that a new event has been added to the builder.

**Required**

func workoutBuilder(HKLiveWorkoutBuilder, didBegin: HKWorkoutActivity)

Tells the delegate that a new workout activity has started.

func workoutBuilder(HKLiveWorkoutBuilder, didEnd: HKWorkoutActivity)

Tells the delegate that the current workout activity has ended.

