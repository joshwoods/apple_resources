

- AVRouting
-  AVCustomRoutingControllerDelegate 

Protocol

# AVCustomRoutingControllerDelegate

A protocol for delegates of a custom routing controller.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+visionOS 1.0+

``` source
protocol AVCustomRoutingControllerDelegate : NSObjectProtocol, Sendable
```

## Topics

### Handling controller events

func customRoutingController(AVCustomRoutingController, handle: AVCustomRoutingEvent, completionHandler: (Bool) -> Void)

Connects to, or disconnects from, a device when a user requests it in the picker.

**Required**

func customRoutingController(AVCustomRoutingController, eventDidTimeOut: AVCustomRoutingEvent)

Tells the delegate when a routing event times out.

func customRoutingController(AVCustomRoutingController, didSelect: AVCustomRoutingActionItem)

Tells the delegate when a user selects a custom item in the route picker.

## Relationships

### Inherits From

- NSObjectProtocol
- Sendable

## See Also

### Media routing

class AVCustomRoutingController

An object that manages the connection from a device to a destination.

class AVCustomRoutingEvent

An object that represents an event that occurs on a route.

class AVCustomRoutingActionItem

An object that represents a custom action item to display in a device route picker.

