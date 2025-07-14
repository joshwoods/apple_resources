

- UIKit
- UIDropInteractionDelegate
-  dropInteraction(\_:sessionDidExit:) 

Instance Method

# dropInteraction(\_:sessionDidExit:)

Tells the delegate the drop session has moved out of the drop interaction’s view.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
optional func dropInteraction(
    _ interaction: UIDropInteraction,
    sessionDidExit session: any UIDropSession
)
```

## Parameters 

`interaction`  

The interaction that called this method.

`session`  

The drop session that has moved out of the interaction’s view.

## See Also

### Tracking the drop movements

func dropInteraction(UIDropInteraction, sessionDidEnter: any UIDropSession)

Tells the delegate the drop session has moved into the drop interaction’s view.

func dropInteraction(UIDropInteraction, sessionDidUpdate: any UIDropSession) -> UIDropProposal

Tells the delegate the drop session has changed.

func dropInteraction(UIDropInteraction, sessionDidEnd: any UIDropSession)

Tells the delegate the drop session has ended.

