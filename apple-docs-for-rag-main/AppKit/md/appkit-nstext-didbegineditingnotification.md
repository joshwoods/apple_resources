

- AppKit
- NSText
-  didBeginEditingNotification 

Type Property

# didBeginEditingNotification

Posted when an `NSText` object begins any operation that changes characters or formatting attributes.

macOS

``` source
class let didBeginEditingNotification: NSNotification.Name
```

## Discussion

The notification object is the notifying `NSText` object. This notification does not contain a `userInfo` dictionary.

## See Also

### Notifications

class let didChangeNotification: NSNotification.Name

Posted after an `NSText` object performs any operation that changes characters or formatting attributes.

class let didEndEditingNotification: NSNotification.Name

Posted when focus leaves an `NSText` object, whether or not any operation has changed characters or formatting attributes.

class let movementUserInfoKey: String

The `userInfo` dictionary key for the didEndEditingNotification notification.

enum NSTextMovement

