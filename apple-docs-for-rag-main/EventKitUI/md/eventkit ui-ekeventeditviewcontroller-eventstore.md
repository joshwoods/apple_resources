

- EventKit UI
- EKEventEditViewController
-  eventStore 

Instance Property

# eventStore

The event store used to save the event.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
var eventStore: EKEventStore! { get set }
```

## Discussion

This property must be set before displaying the view.

## See Also

### Creating and Saving Events

var event: EKEvent?

The event the user creates or edits using this view controller.

