

- UIKit
- UIDragInteractionDelegate
-  dragInteraction(\_:sessionAllowsMoveOperation:) 

Instance Method

# dragInteraction(\_:sessionAllowsMoveOperation:)

Asks the delegate whether the session allows the move operation.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
optional func dragInteraction(
    _ interaction: UIDragInteraction,
    sessionAllowsMoveOperation session: any UIDragSession
) -> Bool
```

## Parameters 

`interaction`  

The interaction that called this method.

`session`  

The drag session that should, or should not, allow the move operation.

## Return Value

true if the session allows moving drag items to the destination view; otherwise false. The default is true if you don’t provide this method.

## Discussion

The UIDropOperation.move operation only applies to drop activities within the same app. Drag items dropped onto another app are always copied.

## See Also

### Restricting the drag behavior

func dragInteraction(UIDragInteraction, sessionIsRestrictedToDraggingApplication: any UIDragSession) -> Bool

Asks the delegate whether the system should restrict the drag session to the app that started the session.

