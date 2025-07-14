

- AVRouting
- AVCustomRoutingControllerDelegate
-  customRoutingController(\_:didSelect:) 

Instance Method

# customRoutingController(\_:didSelect:)

Tells the delegate when a user selects a custom item in the route picker.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+visionOS 1.0+

``` source
optional func customRoutingController(
    _ controller: AVCustomRoutingController,
    didSelect customActionItem: AVCustomRoutingActionItem
)
```

## Parameters 

`controller`  

A custom routing controller.

`customActionItem`  

The selected action item.

## See Also

### Handling controller events

func customRoutingController(AVCustomRoutingController, handle: AVCustomRoutingEvent, completionHandler: (Bool) -> Void)

Connects to, or disconnects from, a device when a user requests it in the picker.

**Required**

func customRoutingController(AVCustomRoutingController, eventDidTimeOut: AVCustomRoutingEvent)

Tells the delegate when a routing event times out.

