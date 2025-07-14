

- UIKit
- UIPointerLockState
-  didChangeNotification 

Type Property

# didChangeNotification

A notification that posts when the value of the locked state for a scene changes.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+visionOS 1.0+

``` source
nonisolated
class let didChangeNotification: NSNotification.Name
```

## Discussion

This notification is sent when the value in the isLocked property changes. The `userInfo` dictionary of the notification contains the sceneUserInfoKey key, which reflects the new value of the isLocked property.

## See Also

### Updating the Lock State

class let sceneUserInfoKey: String

A key that reflects the new locked state.

