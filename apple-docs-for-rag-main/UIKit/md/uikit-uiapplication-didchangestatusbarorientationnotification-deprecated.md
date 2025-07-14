

- UIKit
- UIApplication
-  didChangeStatusBarOrientationNotification Deprecated

Type Property

# didChangeStatusBarOrientationNotification

Posted when the orientation of the app’s user interface changes.

iOS 2.0–13.0DeprecatediPadOS 2.0–13.0DeprecatedMac Catalyst 13.1–13.1Deprecated

``` source
nonisolated
class let didChangeStatusBarOrientationNotification: NSNotification.Name
```

## Discussion

The `userInfo` dictionary contains an NSNumber object that encapsulates a `UIInterfaceOrientation` value (see UIInterfaceOrientation). Use statusBarOrientationUserInfoKey to access this value

## See Also

### Deprecated notifications

class let willChangeStatusBarFrameNotification: NSNotification.Name

Posted when the app is about to change the frame of the status bar.

Deprecated

class let didChangeStatusBarFrameNotification: NSNotification.Name

Posted when the frame of the status bar changes.

Deprecated

class let willChangeStatusBarOrientationNotification: NSNotification.Name

Posted when the app is about to change the orientation of its interface.

Deprecated

