

- HealthKit
- HKWorkoutBuilder
-  addMetadata(\_:completion:) 

Instance Method

# addMetadata(\_:completion:)

Adds metadata to be saved with the workout.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+macOSvisionOS 1.0+watchOS 5.0+

``` source
func addMetadata(
    _ metadata: [String : Any],
    completion: @escaping (Bool, (any Error)?) -> Void
)
```

``` source
func addMetadata(_ metadata: [String : Any]) async throws
```

## See Also

### Adding metadata to the workout

var metadata: [String : Any]

The metadata the builder saves with the workout.

