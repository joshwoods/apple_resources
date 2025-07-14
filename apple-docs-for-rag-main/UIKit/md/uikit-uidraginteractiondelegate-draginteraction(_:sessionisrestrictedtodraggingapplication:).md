

- UIKit
- UIDragInteractionDelegate
-  dragInteraction(\_:sessionIsRestrictedToDraggingApplication:) 

Instance Method

# dragInteraction(\_:sessionIsRestrictedToDraggingApplication:)

Asks the delegate whether the system should restrict the drag session to the app that started the session.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
optional func dragInteraction(
    _ interaction: UIDragInteraction,
    sessionIsRestrictedToDraggingApplication session: any UIDragSession
) -> Bool
```

## Parameters 

`interaction`  

The interaction that called this method.

`session`  

The drag session to restrict or not restrict.

## Return Value

true if you want to restrict the drag session to the app that started it; otherwise false, which is the default if you don’t provide this method.

## Discussion

If you return true and the user attempts to drop the drag items onto another app, the system cancels the session.

Note

The system calls this method only on devices that support dragging across apps.

## See Also

### Restricting the drag behavior

func dragInteraction(UIDragInteraction, sessionAllowsMoveOperation: any UIDragSession) -> Bool

Asks the delegate whether the session allows the move operation.

