

- AVRouting
- AVCustomRoutingController
-  authorizedRoutes 

Instance Property

# authorizedRoutes

A list of authorized routes.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+visionOS 1.0+

``` source
var authorizedRoutes: [AVCustomDeviceRoute] { get }
```

## Discussion

After a user activates a route, it remains authorized for a certain amount of time even if the connection to the route is temporarily unavailable. Your app may reactivate any one of these routes when appropriate, but it needs to inform the system by calling setActive(_:for:).

## See Also

### Managing authorization

class let authorizedRoutesDidChange: NSNotification.Name

A notification the system posts when the list of authorized routes changes.

func invalidateAuthorization(for: AVCustomDeviceRoute)

Revokes an app’s authorization to connect to a route.

