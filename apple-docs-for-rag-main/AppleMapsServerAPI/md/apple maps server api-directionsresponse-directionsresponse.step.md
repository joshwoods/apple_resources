

- Apple Maps Server API
- DirectionsResponse
-  DirectionsResponse.Step 

Object

# DirectionsResponse.Step

An object that represents a step along a route.

Apple Maps Server API 1.2+

``` source
object DirectionsResponse.Step
```

## Properties

`distanceMeters`

`integer`

Total distance covered by the step, in meters.

`durationSeconds`

`integer`

The estimated time to traverse this step, in seconds.

`instructions`

`string`

The localized instruction string for this step that you can use for display purposes.

You can specify the language to receive the response in using the `lang` parameter.

`stepPathIndex`

`integer`

A pointer to this step’s path. The pointer is in the form of an index into the `stepPaths` array contained in a `Route`.

Step paths are self-contained which implies that the last point of a previous step path along a route is the same as the first point of the next step path. Clients are responsible for avoiding duplication when rendering the point.

`transportType`

`string`

A string that indicates the transport type for this step if it’s different from the `transportType` in the route.

Possible Values: `Automobile, Walking`

## See Also

### Steps and routes

object DirectionsResponse.Route

An object that represent the components of a single route.

