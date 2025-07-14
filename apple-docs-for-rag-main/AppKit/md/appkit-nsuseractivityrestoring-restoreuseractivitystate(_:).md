

- AppKit
- NSUserActivityRestoring
-  restoreUserActivityState(\_:) 

Instance Method

# restoreUserActivityState(\_:)

Restores the state necessary to continue the specified user activity.

macOS 10.10+

``` source
@MainActor
func restoreUserActivityState(_ userActivity: NSUserActivity)
```

**Required**

## Parameters 

`userActivity`  

The user activity to continue.

## Discussion

Implement this method to restore an object’s state using the specified user activity. The system calls this method on any responders or documents passed to the `restorationHandler` in application(_:continue:restorationHandler:). The system calls this method on the main thread. Your implementation should use the state data contained in the specified user activity’s userInfo dictionary to restore the object.

On macOS, the system can automatically restore activities managed by NSDocument if you don’t implement application(_:continue:restorationHandler:), or if you return false. When this occurs, the system opens the document using openDocument(withContentsOf:display:completionHandler:), and calls `restoreUserActivityState` on it.

