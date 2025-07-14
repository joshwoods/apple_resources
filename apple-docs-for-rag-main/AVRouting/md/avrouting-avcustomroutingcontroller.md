

- AVRouting
-  AVCustomRoutingController 

Class

# AVCustomRoutingController

An object that manages the connection from a device to a destination.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+visionOS 1.0+

``` source
class AVCustomRoutingController
```

## Overview

A routing controller also informs its delegate object about which routes the user previously authorized, so it can reconnect, if appropriate.

## Topics

### Managing authorization

var authorizedRoutes: [AVCustomDeviceRoute]

A list of authorized routes.

class let authorizedRoutesDidChange: NSNotification.Name

A notification the system posts when the list of authorized routes changes.

func invalidateAuthorization(for: AVCustomDeviceRoute)

Revokes an app’s authorization to connect to a route.

### Configuring route addresses

var knownRouteIPs: [AVCustomRoutingPartialIP]

An array of route addresses known to be on the local network.

class AVCustomRoutingPartialIP

An object that represents a full or partial IP address.

### Activating a route

func isRouteActive(AVCustomDeviceRoute) -> Bool

Returns a Boolean value that indicates whether a route is active.

func setActive(Bool, for: AVCustomDeviceRoute)

Sets the active state of a route.

### Accessing the delegate

var delegate: (any AVCustomRoutingControllerDelegate)?

A delegate object for a routing controller.

### Customizing the user interface

var customActionItems: [AVCustomRoutingActionItem]

An array of custom action items to add to a route picker.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Media routing

protocol AVCustomRoutingControllerDelegate

A protocol for delegates of a custom routing controller.

class AVCustomRoutingEvent

An object that represents an event that occurs on a route.

class AVCustomRoutingActionItem

An object that represents a custom action item to display in a device route picker.

