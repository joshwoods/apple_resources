

- EventKit UI
- EKEventEditViewController
-  event 

Instance Property

# event

The event the user creates or edits using this view controller.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
var event: EKEvent? { get set }
```

## Discussion

If `nil`, creates and adds a new event to the default calendar’s event store. To avoid throwing an exception, ensure that the event is in the specified event store.

## See Also

### Creating and Saving Events

var eventStore: EKEventStore!

The event store used to save the event.

