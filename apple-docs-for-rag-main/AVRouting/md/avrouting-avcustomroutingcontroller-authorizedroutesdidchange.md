

- AVRouting
- AVCustomRoutingController
-  authorizedRoutesDidChange 

Type Property

# authorizedRoutesDidChange

A notification the system posts when the list of authorized routes changes.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+visionOS 1.0+

``` source
class let authorizedRoutesDidChange: NSNotification.Name
```

## See Also

### Managing authorization

var authorizedRoutes: [AVCustomDeviceRoute]

A list of authorized routes.

func invalidateAuthorization(for: AVCustomDeviceRoute)

Revokes an app’s authorization to connect to a route.

