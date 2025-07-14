

- EventKit UI
- EKCalendarChooser
-  delegate 

Instance Property

# delegate

The calendar chooser’s delegate.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.0+visionOS 1.0+

``` source
@MainActor
weak var delegate: (any EKCalendarChooserDelegate)? { get set }
```

## Discussion

This object should conform to EKCalendarChooserDelegate.

## See Also

### Managing Calendar Selection

protocol EKCalendarChooserDelegate

Methods a calendar chooser’s delegate may use to receive notifications.

