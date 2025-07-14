

- AppKit
- NSTextView
-  didChangeTypingAttributesNotification 

Type Property

# didChangeTypingAttributesNotification

Posted when there is a change in the typing attributes within a text view.

macOS

``` source
class let didChangeTypingAttributesNotification: NSNotification.Name
```

## Discussion

This notification is posted, via the textViewDidChangeTypingAttributes(_:) delegate method, whether or not text has changed as a result of the attribute change.

## See Also

### Notifications

class let didChangeSelectionNotification: NSNotification.Name

Posted when the selected range of characters changes.

class let willChangeNotifyingTextViewNotification: NSNotification.Name

Posted when a new text view is established as the text view that sends notifications.

class let didSwitchToNSLayoutManagerNotification: NSNotification.Name

Posted by the framework after switching to using the compatibility mode layout manager.

class let willSwitchToNSLayoutManagerNotification: NSNotification.Name

Posted by the framework before switching to the compatibility mode layout manager.

