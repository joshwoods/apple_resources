

- UIKit
- UIDragInteractionDelegate
-  dragInteraction(\_:sessionForAddingItems:withTouchAt:) 

Instance Method

# dragInteraction(\_:sessionForAddingItems:withTouchAt:)

Asks the delegate which drag session to add drag items to when there is more than one in-progress session.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
optional func dragInteraction(
    _ interaction: UIDragInteraction,
    sessionForAddingItems sessions: [any UIDragSession],
    withTouchAt point: CGPoint
) -> (any UIDragSession)?
```

## Parameters 

`interaction`  

The interaction that called this method.

`sessions`  

An array of in-progress drag sessions.

`point`  

The location of the user’s touch in the view. The touch point is in the view’s coordinate system.

## Return Value

The drag session to add drag items to, or `nil` to continue without adding drag items to any drag session.

## Discussion

If more than one drag session exists, the session used to add drag items may not be apparent to the user. Therefore, by default, no items are added to any session. If you want to change this behavior, implement this method and return the appropriate session. Return `nil` to continue without adding items.

## See Also

### Performing the drag

func dragInteraction(UIDragInteraction, itemsForBeginning: any UIDragSession) -> [UIDragItem]

Asks the delegate for the array of drag items for an impending drag interaction.

**Required**

func dragInteraction(UIDragInteraction, itemsForAddingTo: any UIDragSession, withTouchAt: CGPoint) -> [UIDragItem]

Asks the delegate for the drag items to add to an in-progress drag session, in response to a user gesture to add the items.

