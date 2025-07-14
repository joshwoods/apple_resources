

- Shared With You
- SWCollaborationViewDelegate
-  collaborationViewDidDismissPopover(\_:) 

Instance Method

# collaborationViewDidDismissPopover(\_:)

Notifies the delegate after the system dismisses the popover.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+visionOS 1.0+

``` source
optional func collaborationViewDidDismissPopover(_ collaborationView: SWCollaborationView)
```

## Parameters 

`collaborationView`  

The related `SWCollaborationView`.

## See Also

### Responding to popover activity

func collaborationViewShouldPresentPopover(SWCollaborationView) -> Bool

Asks the delegate whether the system can display the popover.

func collaborationViewWillPresentPopover(SWCollaborationView)

Notifies the delegate before the system presents the popover.

