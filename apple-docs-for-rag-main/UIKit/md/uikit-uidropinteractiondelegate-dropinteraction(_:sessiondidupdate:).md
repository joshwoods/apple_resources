

- UIKit
- UIDropInteractionDelegate
-  dropInteraction(\_:sessionDidUpdate:) 

Instance Method

# dropInteraction(\_:sessionDidUpdate:)

Tells the delegate the drop session has changed.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
optional func dropInteraction(
    _ interaction: UIDropInteraction,
    sessionDidUpdate session: any UIDropSession
) -> UIDropProposal
```

## Parameters 

`interaction`  

The interaction that called this method.

`session`  

The drop session that has changed.

## Return Value

A drop proposal that contains the operation the delegate intends to perform. You may return a proposal containing the UIDropOperation.move operation only if the session’s allowsMoveOperation is true.

## Mentioned in 

Making a view into a drop destination

## Discussion

You must implement this method if the drop interaction’s view can accept drop activities. If you don’t provide this method, the view cannot accept any drop activities.

The interaction calls this method when one of the following happens:

- The session enters the area of the drop interaction’s view.

- The session moves inside the area of the drop interaction’s view.

- The user adds a drag item to the session that within the area of the drop interaction’s view.

To get the location of the drop session after it has moved, call the session’s location(in:) method.

## See Also

### Tracking the drop movements

func dropInteraction(UIDropInteraction, sessionDidEnter: any UIDropSession)

Tells the delegate the drop session has moved into the drop interaction’s view.

func dropInteraction(UIDropInteraction, sessionDidExit: any UIDropSession)

Tells the delegate the drop session has moved out of the drop interaction’s view.

func dropInteraction(UIDropInteraction, sessionDidEnd: any UIDropSession)

Tells the delegate the drop session has ended.

