

- AVRouting
-  AVCustomDeviceRoute 

Class

# AVCustomDeviceRoute

An object that represents a custom device route.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+visionOS 1.0+

``` source
class AVCustomDeviceRoute
```

## Overview

Use the value of a route’s networkEndpoint or bluetoothIdentifier property to establish a connection to a device. Typically, only one of the properties provides a valid value, depending on the type of device. In certain cases, both properties may provide valid values, in which case your app determines which one to use.

## Topics

### Identifying routes

var bluetoothIdentifier: UUID?

An identifier to use to establish a connection to a Bluetooth device.

var networkEndpoint: nw_endpoint_t?

A local or remote endpoint to connect to.

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
- Sendable

## See Also

### Inspecting an event

var route: AVCustomDeviceRoute

A route for the event.

var reason: AVCustomRoutingEventReason

A reason for an event, such as a user request to activate or deactivate a route.

enum AVCustomRoutingEventReason

Values that indicate the reason for a routing event.

