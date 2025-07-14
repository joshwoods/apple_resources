

- HealthKit
- HKWorkoutRouteQuery
-  init(route:dateInterval:dataHandler:) 

Initializer

# init(route:dateInterval:dataHandler:)

Creates a new query to access the location data associated with a workout route during the specified date interval.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+visionOS 1.0+watchOS 9.0+

``` source
init(
    route workoutRoute: HKWorkoutRoute,
    dateInterval: DateInterval,
    dataHandler: @escaping (HKWorkoutRouteQuery, [CLLocation]?, Bool, (any Error)?) -> Void
)
```

## Parameters 

`workoutRoute`  

The workout route that contains the location data.

`dateInterval`  

The date interval for the requested location data. If the date interval doesn’t overlap with the specified workout, this query returns an empty array.

If the date interval only partially overlaps the specified workout, the query only returns location data from the overlapping time period.

`dataHandler`  

A block that the system calls each time it returns a batch of location data. The system may call this block more than once.

The system passes this block the following parameters:

`query`  
The query that returns the location data.

`routeData`  
A batch of location data, or `nil` if an error has occurred.

`done`  
A Boolean value that indicates whether the query is complete. It is true if all the location data has been returned. If one or more additional batches of data are still pending, it is false.

`error`  
An object that describes the error, if an error has occurred; otherwise, `nil`.

## See Also

### Creating route queries

init(route: HKWorkoutRoute, dataHandler: (HKWorkoutRouteQuery, [CLLocation]?, Bool, (any Error)?) -> Void)

Creates a new query to access the location data associated with a workout route.

