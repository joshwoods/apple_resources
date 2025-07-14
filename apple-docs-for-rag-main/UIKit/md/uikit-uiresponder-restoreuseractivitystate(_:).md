

- UIKit
- UIResponder
-  restoreUserActivityState(\_:) 

Instance Method

# restoreUserActivityState(\_:)

Restores the state needed to continue the given user activity.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
func restoreUserActivityState(_ activity: NSUserActivity)
```

## Parameters 

`activity`  

The user activity to be continued.

## Discussion

Subclasses override this method to restore the responder’s state with the given user activity. The system calls it on any objects passed to the restoration handler given to application(_:continue:restorationHandler:). The override should use the state data contained in the given user activity’s `userInfo` dictionary to restore the object.

You may also call this method directly if the app delegate chooses not to use the restoration handler.

## See Also

### Supporting user activities

var userActivity: NSUserActivity?

An object encapsulating a user activity supported by this responder.

func updateUserActivityState(NSUserActivity)

Updates the state of the given user activity.

