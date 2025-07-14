

- AppKit
- NSTextView
-  willSwitchToNSLayoutManagerNotification 

Type Property

# willSwitchToNSLayoutManagerNotification

Posted by the framework before switching to the compatibility mode layout manager.

macOS 12.0+

``` source
class let willSwitchToNSLayoutManagerNotification: NSNotification.Name
```

## See Also

### Notifications

class let didChangeSelectionNotification: NSNotification.Name

Posted when the selected range of characters changes.

class let willChangeNotifyingTextViewNotification: NSNotification.Name

Posted when a new text view is established as the text view that sends notifications.

class let didChangeTypingAttributesNotification: NSNotification.Name

Posted when there is a change in the typing attributes within a text view.

class let didSwitchToNSLayoutManagerNotification: NSNotification.Name

Posted by the framework after switching to using the compatibility mode layout manager.

