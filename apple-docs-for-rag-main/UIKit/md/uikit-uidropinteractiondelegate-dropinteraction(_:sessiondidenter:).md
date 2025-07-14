

- UIKit
- UIDropInteractionDelegate
-  dropInteraction(\_:sessionDidEnter:) 

Instance Method

# dropInteraction(\_:sessionDidEnter:)

Tells the delegate the drop session has moved into the drop interaction’s view.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
optional func dropInteraction(
    _ interaction: UIDropInteraction,
    sessionDidEnter session: any UIDropSession
)
```

## Parameters 

`interaction`  

The interaction that called this method.

`session`  

The drop session that has moved into the interaction’s view.

## Mentioned in 

Making a view into a drop destination

## See Also

### Tracking the drop movements

func dropInteraction(UIDropInteraction, sessionDidUpdate: any UIDropSession) -> UIDropProposal

Tells the delegate the drop session has changed.

func dropInteraction(UIDropInteraction, sessionDidExit: any UIDropSession)

Tells the delegate the drop session has moved out of the drop interaction’s view.

func dropInteraction(UIDropInteraction, sessionDidEnd: any UIDropSession)

Tells the delegate the drop session has ended.

