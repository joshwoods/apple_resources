

- HealthKit
- HKLiveWorkoutDataSource
-  typesToCollect 

Instance Property

# typesToCollect

The quantity type samples that the data source automatically sends to the workout builder.

macOSwatchOS 5.0+

``` source
var typesToCollect: Set { get }
```

## Discussion

Apple Watch automatically collects the listed data types and sends the data to the workout builder. The available data types vary depending on the user’s settings and the workout configuration, and can include types like basalEnergyBurned, activeEnergyBurned, heartRate, distanceWalkingRunning, distanceCycling, distanceSwimming, or distanceWheelchair.

To monitor this data, add a delegate to the session’s HKLiveWorkoutBuilder object, and implement its workoutBuilder(_:didCollectDataOf:) method.

## See Also

### Creating a live data source

init(healthStore: HKHealthStore, workoutConfiguration: HKWorkoutConfiguration?)

Creates a new data source based on the provided workout configuration.

