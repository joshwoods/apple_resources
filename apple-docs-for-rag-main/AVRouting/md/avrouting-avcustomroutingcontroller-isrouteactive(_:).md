

- AVRouting
- AVCustomRoutingController
-  isRouteActive(\_:) 

Instance Method

# isRouteActive(\_:)

Returns a Boolean value that indicates whether a route is active.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+visionOS 1.0+

``` source
func isRouteActive(_ route: AVCustomDeviceRoute) -> Bool
```

## Parameters 

`route`  

A route for determining its active state.

## Return Value

true if the route is in an active state; otherwise, false.

## See Also

### Activating a route

func setActive(Bool, for: AVCustomDeviceRoute)

Sets the active state of a route.

