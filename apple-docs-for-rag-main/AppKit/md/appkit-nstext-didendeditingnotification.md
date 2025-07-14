

- AppKit
- NSText
-  didEndEditingNotification 

Type Property

# didEndEditingNotification

Posted when focus leaves an `NSText` object, whether or not any operation has changed characters or formatting attributes.

macOS

``` source
class let didEndEditingNotification: NSNotification.Name
```

## Discussion

The notification object is the notifying `NSText` object. The `userInfo` dictionary contains the following information:

| Key | Value |
|----|----|
| movementUserInfoKey | One of the values in NSTextMovement. |

| Key | Value |
|----|----|
| `@"NSTextMovement"` | Possible movement code values are described in Movement Codes. |

Note

It is common for didEndEditingNotification to be sent without a matching didBeginEditingNotification. The begin notification is only sent if the user actually makes changes (that is, types something or changes formatting attributes). However, the end notification is sent when focus leaves the text view, regardless of whether there was a change.

This distinction enables an application to know whether the user actually made a change to the text or just clicked in the text view and then clicked outside it. In both cases, didEndEditingNotification is sent, but to tell the difference, the application can listen for didBeginEditingNotification.

## See Also

### Notifications

class let didBeginEditingNotification: NSNotification.Name

Posted when an `NSText` object begins any operation that changes characters or formatting attributes.

class let didChangeNotification: NSNotification.Name

Posted after an `NSText` object performs any operation that changes characters or formatting attributes.

class let movementUserInfoKey: String

The `userInfo` dictionary key for the didEndEditingNotification notification.

enum NSTextMovement

