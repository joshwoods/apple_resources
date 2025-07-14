

- HealthKit
- HKWorkoutRouteBuilder
-  insertRouteData(\_:completion:) 

Instance Method

# insertRouteData(\_:completion:)

Adds route data to the builder.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.0+macOS 13.0+visionOS 1.0+watchOS 4.0+

``` source
func insertRouteData(
    _ routeData: [CLLocation],
    completion: @escaping (Bool, (any Error)?) -> Void
)
```

``` source
func insertRouteData(_ routeData: [CLLocation]) async throws
```

## Parameters 

`routeData`  

An array containing one or more location objects.

`completion`  

A block called after the system adds the collection data to the builder. The system passes the block the following parameters:

`success`  
A Boolean value that indicates whether the builder successfully received the route data.

`error`  
An object that describes the error, if an error has occurred; otherwise, `nil`.

## Mentioned in 

Creating a workout route

## Discussion

Use this method to asynchronously add one or more CLLocation objects to the series. The CLLocation objects may be inserted in any order; the builder sorts them by date when finalizing the route.

## See Also

### Building the route

func finishRoute(with: HKWorkout, metadata: [String : Any]?, completion: (HKWorkoutRoute?, (any Error)?) -> Void)

Creates, saves, and associates the route with the provided workout.

func addMetadata([String : Any], completion: (Bool, (any Error)?) -> Void)

Adds metadata to the builder.

