

- HealthKit
- HKWorkoutBuilder
-  metadata 

Instance Property

# metadata

The metadata the builder saves with the workout.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+macOSvisionOS 1.0+watchOS 5.0+

``` source
var metadata: [String : Any] { get }
```

## See Also

### Adding metadata to the workout

func addMetadata([String : Any], completion: (Bool, (any Error)?) -> Void)

Adds metadata to be saved with the workout.

