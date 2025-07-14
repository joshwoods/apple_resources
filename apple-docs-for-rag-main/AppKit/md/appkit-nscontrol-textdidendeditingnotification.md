

- AppKit
- NSControl
-  textDidEndEditingNotification 

Type Property

# textDidEndEditingNotification

Sent when a control with editable cells ends an editing session.

macOS

``` source
class let textDidEndEditingNotification: NSNotification.Name
```

## Discussion

The field editor of the edited cell originally sends an textDidEndEditingNotification to the control, which passes it on in this form to its delegate. The notification object is the `NSControl` object posting the notification. The `userInfo` dictionary contains the following information:

| Key               | Value                          |
|-------------------|--------------------------------|
| `“NSFieldEditor”` | The edited cell’s field editor |

See the controlTextDidEndEditing: method for details. The system posts this notification on the main actor.

## See Also

### Control-Editing Notifications

class let textDidBeginEditingNotification: NSNotification.Name

Sent when a control with editable cells begins an edit session.

class let textDidChangeNotification: NSNotification.Name

Sent when the text in the receiving control changes.

