

- Shared With You
- SWCollaborationViewDelegate
-  collaborationViewWillPresentPopover(\_:) 

Instance Method

# collaborationViewWillPresentPopover(\_:)

Notifies the delegate before the system presents the popover.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+visionOS 1.0+

``` source
optional func collaborationViewWillPresentPopover(_ collaborationView: SWCollaborationView)
```

## Parameters 

`collaborationView`  

The related `SWCollaborationView`.

## See Also

### Responding to popover activity

func collaborationViewShouldPresentPopover(SWCollaborationView) -> Bool

Asks the delegate whether the system can display the popover.

func collaborationViewDidDismissPopover(SWCollaborationView)

Notifies the delegate after the system dismisses the popover.

