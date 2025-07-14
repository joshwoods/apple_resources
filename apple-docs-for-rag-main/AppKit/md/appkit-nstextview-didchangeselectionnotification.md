

- AppKit
- NSTextView
-  didChangeSelectionNotification 

Type Property

# didChangeSelectionNotification

Posted when the selected range of characters changes.

macOS

``` source
class let didChangeSelectionNotification: NSNotification.Name
```

## Discussion

`NSTextView` posts this notification whenever setSelectedRange(_:affinity:stillSelecting:) is invoked, either directly or through the many methods (mouseDown(with:), selectAll(_:), and so on) that invoke it indirectly. When the user is selecting text, this notification is posted only once, at the end of the selection operation. The text view’s delegate receives a textViewDidChangeSelection(_:) message when this notification is posted.

The notification object is the notifying text view. The `userInfo` dictionary contains the following information:

| Key | Value |
|----|----|
| `@"NSOldSelectedCharacterRange"` | An `NSValue` object containing an `NSRange` structure with the originally selected range. |

## See Also

### Notifications

class let willChangeNotifyingTextViewNotification: NSNotification.Name

Posted when a new text view is established as the text view that sends notifications.

class let didChangeTypingAttributesNotification: NSNotification.Name

Posted when there is a change in the typing attributes within a text view.

class let didSwitchToNSLayoutManagerNotification: NSNotification.Name

Posted by the framework after switching to using the compatibility mode layout manager.

class let willSwitchToNSLayoutManagerNotification: NSNotification.Name

Posted by the framework before switching to the compatibility mode layout manager.

