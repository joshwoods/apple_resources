

- HealthKit
- HKWorkoutRouteQuery
-  init(route:dataHandler:) 

Initializer

# init(route:dataHandler:)

Creates a new query to access the location data associated with a workout route.

iOSiPadOSMac CatalystmacOSvisionOSwatchOS

``` source
init(
    route workoutRoute: HKWorkoutRoute,
    dataHandler: @escaping (HKWorkoutRouteQuery, [CLLocation]?, Bool, (any Error)?) -> Void
)
```

## Parameters 

`workoutRoute`  

The workout route containing the location data.

`dataHandler`  

A block called each time the system returns a batch of location data. This block may be called one or more times.

The block is passed the following parameters:

`query`  
The query that returns the location data.

`routeData`  
A batch of location data, or `nil` if an error has occurred.

`done`  
A Boolean value that indicates whether the query is complete. It is true if all the location data has been returned. If one or more additional batches of data are still pending, it is false.

`error`  
An object that describes the error, if an error has occurred; otherwise, `nil`.

## Return Value

A newly initialized route query.

## See Also

### Creating route queries

init(route: HKWorkoutRoute, dateInterval: DateInterval, dataHandler: (HKWorkoutRouteQuery, [CLLocation]?, Bool, (any Error)?) -> Void)

Creates a new query to access the location data associated with a workout route during the specified date interval.

