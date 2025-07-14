

- HomeKit
- HMEventTrigger
-  updateEndEvents(\_:completionHandler:) 

Instance Method

# updateEndEvents(\_:completionHandler:)

Updates the set of end events associated with the event trigger.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
func updateEndEvents(
    _ endEvents: [HMEvent],
    completionHandler completion: @escaping ((any Error)?) -> Void
)
```

``` source
func updateEndEvents(_ endEvents: [HMEvent]) async throws
```

## Parameters 

`endEvents`  

An array of events that replaces the end events on the trigger.

`completion`  

A block that executes after processing the request.

The block takes the following parameter:

error  
If the request was successful, the value of `error` is `nil`; otherwise, the value provides more information about the request status.

## See Also

### Restoring the previous scene after an event

var endEvents: [HMEvent]

The events associated with the end of scene represented by this trigger.

