

- EventKit UI
- EKEventViewController
-  delegate 

Instance Property

# delegate

The event view controller’s delegate.

iOS 4.2+iPadOS 4.2+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
weak var delegate: (any EKEventViewDelegate)? { get set }
```

## See Also

### Dismissing the Event Interface

protocol EKEventViewDelegate

Delegates used to display details for calendar events.

