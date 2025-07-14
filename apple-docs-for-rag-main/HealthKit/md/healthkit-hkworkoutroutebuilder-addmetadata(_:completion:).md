

- HealthKit
- HKWorkoutRouteBuilder
-  addMetadata(\_:completion:) 

Instance Method

# addMetadata(\_:completion:)

Adds metadata to the builder.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.0+macOS 13.0+visionOS 1.0+watchOS 4.0+

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

### Building the route

func finishRoute(with: HKWorkout, metadata: [String : Any]?, completion: (HKWorkoutRoute?, (any Error)?) -> Void)

Creates, saves, and associates the route with the provided workout.

func insertRouteData([CLLocation], completion: (Bool, (any Error)?) -> Void)

Adds route data to the builder.

