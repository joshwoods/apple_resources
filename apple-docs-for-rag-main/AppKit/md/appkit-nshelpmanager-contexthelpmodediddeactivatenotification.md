

- AppKit
- NSHelpManager
-  contextHelpModeDidDeactivateNotification 

Type Property

# contextHelpModeDidDeactivateNotification

Posted when the application exits context-sensitive help mode. This happens when the user clicks the mouse button while the cursor is anywhere on the screen after displaying a context-sensitive help topic.

macOS

``` source
class let contextHelpModeDidDeactivateNotification: NSNotification.Name
```

## Discussion

The notification object is the help manager. This notification does not contain a `userInfo` dictionary.

## See Also

### Notifications

class let contextHelpModeDidActivateNotification: NSNotification.Name

Posted when the application enters context-sensitive help mode. This typically happens when the user holds down the Help key.

