

- UIKit
- UIPointerLockState
-  sceneUserInfoKey 

Type Property

# sceneUserInfoKey

A key that reflects the new locked state.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+visionOS 1.0+

``` source
nonisolated
class let sceneUserInfoKey: String
```

## Discussion

The `userInfo` dictionary of the notification contains the sceneUserInfoKey key, which reflects the new value of the isLocked property.

## See Also

### Updating the Lock State

class let didChangeNotification: NSNotification.Name

A notification that posts when the value of the locked state for a scene changes.

