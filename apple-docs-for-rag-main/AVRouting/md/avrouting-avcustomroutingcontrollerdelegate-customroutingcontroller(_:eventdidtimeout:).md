

- AVRouting
- AVCustomRoutingControllerDelegate
-  customRoutingController(\_:eventDidTimeOut:) 

Instance Method

# customRoutingController(\_:eventDidTimeOut:)

Tells the delegate when a routing event times out.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+visionOS 1.0+

``` source
optional func customRoutingController(
    _ controller: AVCustomRoutingController,
    eventDidTimeOut event: AVCustomRoutingEvent
)
```

## Parameters 

`controller`  

A custom routing controller.

`event`  

An event that times out.

## Discussion

Adopt this method to clean up any in-progress connection attempts.

## See Also

### Handling controller events

func customRoutingController(AVCustomRoutingController, handle: AVCustomRoutingEvent, completionHandler: (Bool) -> Void)

Connects to, or disconnects from, a device when a user requests it in the picker.

**Required**

func customRoutingController(AVCustomRoutingController, didSelect: AVCustomRoutingActionItem)

Tells the delegate when a user selects a custom item in the route picker.

