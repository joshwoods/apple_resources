

- EventKit UI
- EKEventEditViewController
-  editViewDelegate 

Instance Property

# editViewDelegate

The delegate to notify when editing an event.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
weak var editViewDelegate: (any EKEventEditViewDelegate)? { get set }
```

## See Also

### Managing the Event Editing Interface

protocol EKEventEditViewDelegate

A notification sent to the delegate when the user finishes editing an event.

