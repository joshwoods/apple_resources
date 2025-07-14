

- UIKit
- UIUserActivityRestoring
-  restoreUserActivityState(\_:) 

Instance Method

# restoreUserActivityState(\_:)

Restores the state necessary to continue the specified user activity.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
func restoreUserActivityState(_ userActivity: NSUserActivity)
```

**Required**

## Parameters 

`userActivity`  

The user activity to continue.

## Discussion

Implement this method to restore an object’s state using the specified user activity. The system calls this method on any objects passed to the restoration handler in application(_:continue:restorationHandler:). Your implementation should use the state data contained in the specified user activity’s userInfo dictionary to restore the object.

