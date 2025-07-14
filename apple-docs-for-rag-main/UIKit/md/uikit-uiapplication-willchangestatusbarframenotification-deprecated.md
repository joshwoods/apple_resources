

- UIKit
- UIApplication
-  willChangeStatusBarFrameNotification Deprecated

Type Property

# willChangeStatusBarFrameNotification

Posted when the app is about to change the frame of the status bar.

iOS 2.0–13.0DeprecatediPadOS 2.0–13.0DeprecatedMac Catalyst 13.1–13.1Deprecated

``` source
nonisolated
class let willChangeStatusBarFrameNotification: NSNotification.Name
```

## Discussion

The `userInfo` dictionary contains an NSValue object that encapsulates a CGRect structure expressing the location and size of the new status bar frame. Use statusBarFrameUserInfoKey to access this value.

## See Also

### Deprecated notifications

class let didChangeStatusBarFrameNotification: NSNotification.Name

Posted when the frame of the status bar changes.

Deprecated

class let willChangeStatusBarOrientationNotification: NSNotification.Name

Posted when the app is about to change the orientation of its interface.

Deprecated

class let didChangeStatusBarOrientationNotification: NSNotification.Name

Posted when the orientation of the app’s user interface changes.

Deprecated

