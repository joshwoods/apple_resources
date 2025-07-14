

- Shared With You
- SWCollaborationViewDelegate
-  collaborationViewShouldPresentPopover(\_:) 

Instance Method

# collaborationViewShouldPresentPopover(\_:)

Asks the delegate whether the system can display the popover.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+visionOS 1.0+

``` source
optional func collaborationViewShouldPresentPopover(_ collaborationView: SWCollaborationView) -> Bool
```

## Parameters 

`collaborationView`  

The related `SWCollaborationView`.

## Return Value

`true` if the system should present the popover; otherwise `false`.

## See Also

### Responding to popover activity

func collaborationViewDidDismissPopover(SWCollaborationView)

Notifies the delegate after the system dismisses the popover.

func collaborationViewWillPresentPopover(SWCollaborationView)

Notifies the delegate before the system presents the popover.

