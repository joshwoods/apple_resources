

- UIKit
- UICollectionViewDelegate
-  collectionView(\_:contextMenuConfiguration:highlightPreviewForItemAt:) 

Instance Method

# collectionView(\_:contextMenuConfiguration:highlightPreviewForItemAt:)

Asks the delegate for a preview of the item at the specified index path when a context-menu interaction begins.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+tvOS 17.0+visionOS 1.0+

``` source
@MainActor
optional func collectionView(
    _ collectionView: UICollectionView,
    contextMenuConfiguration configuration: UIContextMenuConfiguration,
    highlightPreviewForItemAt indexPath: IndexPath
) -> UITargetedPreview?
```

## Parameters 

`collectionView`  

The collection view containing the item.

`configuration`  

The configuration of the menu to present if the interaction proceeds.

`indexPath`  

The index path of the item where the interaction occurs.

## Return Value

A targeted preview object corresponding to the item at the index path to use during the menu’s highlight and presentation animation.

## Discussion

The system calls this method when a context-menu interaction begins. Implement this method to override the default highlight preview that the collection view generates for the item at `indexPath`.

## See Also

### Managing context menus

Adding context menus in your app

Provide quick access to useful actions by adding context menus to your iOS app.

func collectionView(UICollectionView, willDisplayContextMenu: UIContextMenuConfiguration, animator: (any UIContextMenuInteractionAnimating)?)

Informs the delegate when a context menu will appear.

func collectionView(UICollectionView, willEndContextMenuInteraction: UIContextMenuConfiguration, animator: (any UIContextMenuInteractionAnimating)?)

Informs the delegate when a context menu will disappear.

func collectionView(UICollectionView, willPerformPreviewActionForMenuWith: UIContextMenuConfiguration, animator: any UIContextMenuInteractionCommitAnimating)

Informs the delegate when a user triggers a commit by tapping the preview.

func collectionView(UICollectionView, contextMenuConfigurationForItemsAt: [IndexPath], point: CGPoint) -> UIContextMenuConfiguration?

Asks the delegate for a context-menu configuration for the items at the specified index paths.

func collectionView(UICollectionView, contextMenuConfiguration: UIContextMenuConfiguration, dismissalPreviewForItemAt: IndexPath) -> UITargetedPreview?

Asks the delegate for a preview of the item at the specified index path when a context-menu interaction ends.

