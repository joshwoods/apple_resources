

- AVRouting
- AVCustomRoutingControllerDelegate
-  customRoutingController(\_:handle:completionHandler:) 

Instance Method

# customRoutingController(\_:handle:completionHandler:)

Connects to, or disconnects from, a device when a user requests it in the picker.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+visionOS 1.0+

``` source
func customRoutingController(
    _ controller: AVCustomRoutingController,
    handle event: AVCustomRoutingEvent,
    completionHandler: @escaping (Bool) -> Void
)
```

``` source
func customRoutingController(
    _ controller: AVCustomRoutingController,
    handle event: AVCustomRoutingEvent
) async -> Bool
```

**Required**

## Parameters 

`controller`  

A custom routing controller.

`event`  

The routing event to handle.

`completionHandler`  

A completion handler to call after processing the event. Pass true to the completion handler if the activation, reactivation, or deactivation of the route succeeds, and false, otherwise.

## Discussion

Important

You can call this method from synchronous code using a completion handler, as shown on this page, or you can call it as an asynchronous method that has the following declaration:

```
func customRoutingController(_ controller: AVCustomRoutingController, handle event: AVCustomRoutingEvent) async -> Bool
```

For information about concurrency and asynchronous code in Swift, see Calling Objective-C APIs Asynchronously.

## See Also

### Handling controller events

func customRoutingController(AVCustomRoutingController, eventDidTimeOut: AVCustomRoutingEvent)

Tells the delegate when a routing event times out.

func customRoutingController(AVCustomRoutingController, didSelect: AVCustomRoutingActionItem)

Tells the delegate when a user selects a custom item in the route picker.

