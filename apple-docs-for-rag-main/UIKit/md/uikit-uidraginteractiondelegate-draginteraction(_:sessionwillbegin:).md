

- UIKit
- UIDragInteractionDelegate
-  dragInteraction(\_:sessionWillBegin:) 

Instance Method

# dragInteraction(\_:sessionWillBegin:)

Tells the delegate the lift animation has finished and the user is starting to move the items across the screen.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
optional func dragInteraction(
    _ interaction: UIDragInteraction,
    sessionWillBegin session: any UIDragSession
)
```

## Parameters 

`interaction`  

The interaction that called this method.

`session`  

The current drag session.

## Discussion

Implement this method when you need to perform some action after the user starts dragging the items; for instance, dimming the view to show that its contents are being dragged.

## See Also

### Monitoring drag progress

func dragInteraction(UIDragInteraction, session: any UIDragSession, willAdd: [UIDragItem], for: UIDragInteraction)

Tells the delegate an interaction is about to add items to a drag session.

func dragInteraction(UIDragInteraction, sessionDidMove: any UIDragSession)

Tells the delegate the user moved the drag items to a new location on the screen.

func dragInteraction(UIDragInteraction, session: any UIDragSession, willEndWith: UIDropOperation)

Tells the delegate the drag activity will end with the specified operation.

func dragInteraction(UIDragInteraction, session: any UIDragSession, didEndWith: UIDropOperation)

Tells the delegate the drag activity and its related animations have finished.

func dragInteraction(UIDragInteraction, sessionDidTransferItems: any UIDragSession)

Tells the delegate the destination view has received the data for the drag items.

