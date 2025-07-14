

- AVRouting
- AVCustomRoutingController
-  setActive(\_:for:) 

Instance Method

# setActive(\_:for:)

Sets the active state of a route.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+visionOS 1.0+

``` source
func setActive(
    _ active: Bool,
    for route: AVCustomDeviceRoute
)
```

## Parameters 

`active`  

A Boolean value that indicates whether the route is active.

`route`  

A route to change the active state for.

## Discussion

Set the value to false if the connection to the route becomes unavailable, and set it to true after you reestablish the connection.

## See Also

### Activating a route

func isRouteActive(AVCustomDeviceRoute) -> Bool

Returns a Boolean value that indicates whether a route is active.

