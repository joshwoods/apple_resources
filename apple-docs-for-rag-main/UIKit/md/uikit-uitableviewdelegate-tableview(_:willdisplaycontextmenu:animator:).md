

- UIKit
- UITableViewDelegate
-  tableView(\_:willDisplayContextMenu:animator:) 

Instance Method

# tableView(\_:willDisplayContextMenu:animator:)

Informs the delegate when a context menu will appear.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+tvOS 17.0+visionOS 1.0+

``` source
@MainActor
optional func tableView(
    _ tableView: UITableView,
    willDisplayContextMenu configuration: UIContextMenuConfiguration,
    animator: (any UIContextMenuInteractionAnimating)?
)
```

## Parameters 

`tableView`  

The table view informing the delegate of this event.

`configuration`  

The configuration of the menu to display.

`animator`  

The animations to run alongside the appearance transition.

## See Also

### Managing context menus

Adding context menus in your app

Provide quick access to useful actions by adding context menus to your iOS app.

func tableView(UITableView, contextMenuConfigurationForRowAt: IndexPath, point: CGPoint) -> UIContextMenuConfiguration?

Returns a context menu configuration for the row at a point.

func tableView(UITableView, previewForDismissingContextMenuWithConfiguration: UIContextMenuConfiguration) -> UITargetedPreview?

Returns the destination view when dismissing a context menu.

func tableView(UITableView, previewForHighlightingContextMenuWithConfiguration: UIContextMenuConfiguration) -> UITargetedPreview?

Returns a view to override the default preview the table view created.

func tableView(UITableView, willEndContextMenuInteraction: UIContextMenuConfiguration, animator: (any UIContextMenuInteractionAnimating)?)

Informs the delegate when a context menu will disappear.

func tableView(UITableView, willPerformPreviewActionForMenuWith: UIContextMenuConfiguration, animator: any UIContextMenuInteractionCommitAnimating)

Informs the delegate when a user triggers a commit by tapping the preview.

