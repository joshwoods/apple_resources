

- AppKit
- NSText
-  movementUserInfoKey 

Type Property

# movementUserInfoKey

The `userInfo` dictionary key for the didEndEditingNotification notification.

macOS 10.13+

``` source
class let movementUserInfoKey: String
```

## See Also

### Notifications

class let didBeginEditingNotification: NSNotification.Name

Posted when an `NSText` object begins any operation that changes characters or formatting attributes.

class let didChangeNotification: NSNotification.Name

Posted after an `NSText` object performs any operation that changes characters or formatting attributes.

class let didEndEditingNotification: NSNotification.Name

Posted when focus leaves an `NSText` object, whether or not any operation has changed characters or formatting attributes.

enum NSTextMovement

