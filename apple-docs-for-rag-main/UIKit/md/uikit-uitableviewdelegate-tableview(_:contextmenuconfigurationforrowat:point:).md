

- UIKit
- UITableViewDelegate
-  tableView(\_:contextMenuConfigurationForRowAt:point:) 

Instance Method

# tableView(\_:contextMenuConfigurationForRowAt:point:)

Returns a context menu configuration for the row at a point.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+tvOS 17.0+visionOS 1.0+

``` source
@MainActor
optional func tableView(
    _ tableView: UITableView,
    contextMenuConfigurationForRowAt indexPath: IndexPath,
    point: CGPoint
) -> UIContextMenuConfiguration?
```

## Parameters 

`tableView`  

The table view containing the row.

`indexPath`  

The index path of the row.

`point`  

The location of the interaction in the table view’s coordinate space.

## Return Value

A context menu configuration for the `indexPath`.

## Discussion

Use this method to provide a UIContextMenuConfiguration describing the menu to present. Return `nil` to prevent the interaction from beginning. Return an empty configuration to begin the interaction and then fail with a cancellation effect. Use the empty configuration to indicate to users that it’s possible for this element to present a menu, but that there are no actions to present at this time.

## See Also

### Managing context menus

Adding context menus in your app

Provide quick access to useful actions by adding context menus to your iOS app.

func tableView(UITableView, previewForDismissingContextMenuWithConfiguration: UIContextMenuConfiguration) -> UITargetedPreview?

Returns the destination view when dismissing a context menu.

func tableView(UITableView, previewForHighlightingContextMenuWithConfiguration: UIContextMenuConfiguration) -> UITargetedPreview?

Returns a view to override the default preview the table view created.

func tableView(UITableView, willDisplayContextMenu: UIContextMenuConfiguration, animator: (any UIContextMenuInteractionAnimating)?)

Informs the delegate when a context menu will appear.

func tableView(UITableView, willEndContextMenuInteraction: UIContextMenuConfiguration, animator: (any UIContextMenuInteractionAnimating)?)

Informs the delegate when a context menu will disappear.

func tableView(UITableView, willPerformPreviewActionForMenuWith: UIContextMenuConfiguration, animator: any UIContextMenuInteractionCommitAnimating)

Informs the delegate when a user triggers a commit by tapping the preview.

