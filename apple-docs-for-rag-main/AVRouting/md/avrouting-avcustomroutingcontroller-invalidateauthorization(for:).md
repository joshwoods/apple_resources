

- AVRouting
- AVCustomRoutingController
-  invalidateAuthorization(for:) 

Instance Method

# invalidateAuthorization(for:)

Revokes an app’s authorization to connect to a route.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+visionOS 1.0+

``` source
func invalidateAuthorization(for route: AVCustomDeviceRoute)
```

## Parameters 

`route`  

The route to invalidate authorization for.

## Discussion

The route only becomes authorized again if the user selects it using the route picker.

## See Also

### Managing authorization

var authorizedRoutes: [AVCustomDeviceRoute]

A list of authorized routes.

class let authorizedRoutesDidChange: NSNotification.Name

A notification the system posts when the list of authorized routes changes.

