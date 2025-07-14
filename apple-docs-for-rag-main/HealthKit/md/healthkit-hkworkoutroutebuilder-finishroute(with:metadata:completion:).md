

- HealthKit
- HKWorkoutRouteBuilder
-  finishRoute(with:metadata:completion:) 

Instance Method

# finishRoute(with:metadata:completion:)

Creates, saves, and associates the route with the provided workout.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.0+macOS 13.0+visionOS 1.0+watchOS 4.0+

``` source
func finishRoute(
    with workout: HKWorkout,
    metadata: [String : Any]?,
    completion: @escaping (HKWorkoutRoute?, (any Error)?) -> Void
)
```

``` source
func finishRoute(
    with workout: HKWorkout,
    metadata: [String : Any]?
) async throws -> HKWorkoutRoute
```

## Parameters 

`workout`  

The workout to associate with the route. You must have already saved this workout to the HealthKit store.

`metadata`  

The metadata dictionary can contain extra information describing this sample. The dictionary’s keys are all NSString objects. The values may be HKQuantity, NSString, NSNumber, or NSDate objects. For a complete list of predefined metadata keys, see Metadata Keys.

Using predefined keys helps facilitate sharing data between apps; however, you are also encouraged to create your own custom keys as needed to extend the HealthKit quantity sample’s capabilities.

`completion`  

A block called after the system has saved the route data. The system passes the block the following parameters:

`workoutRoute`  
The workout route, or `nil` if an error occurred. If successful, the system has already associated the route with the provided workout and saved it to the HealthKit store.

`error`  
An object that describes the error, if an error has occurred; otherwise, `nil`.

## Mentioned in 

Creating a workout route

## Discussion

Call this method after adding all the route data to the builder. The builder creates the route and saves it to the HealthKit store. It also associates the route with the provided workout. You cannot associate the route with another workout.

Note

You must call finishRoute(with:metadata:completion:) before the system deallocates the builder. Failure to do so results in a loss of all route data added to the builder.

This method fails if you haven’t added any location data to the builder. The completion handler returns an error and `nil` for the route.

Additionally, this method invalidates the builder. Any further calls to the builder returns an error. To subsequently access the workout route, use a query (for example, an HKSampleQuery object).

## See Also

### Building the route

func insertRouteData([CLLocation], completion: (Bool, (any Error)?) -> Void)

Adds route data to the builder.

func addMetadata([String : Any], completion: (Bool, (any Error)?) -> Void)

Adds metadata to the builder.

