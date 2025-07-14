

- UIKit
- UICollectionViewDelegate
-  collectionView(\_:willDisplayContextMenu:animator:) 

Instance Method

# collectionView(\_:willDisplayContextMenu:animator:)

Informs the delegate when a context menu will appear.

iOS 13.2+iPadOS 13.2+Mac Catalyst 13.2+tvOS 17.0+visionOS 1.0+

``` source
@MainActor
optional func collectionView(
    _ collectionView: UICollectionView,
    willDisplayContextMenu configuration: UIContextMenuConfiguration,
    animator: (any UIContextMenuInteractionAnimating)?
)
```

## Parameters 

`collectionView`  

The collection view that informs the delegate of this event.

`configuration`  

The configuration of the menu to display.

`animator`  

The animations to run alongside the appearance transition.

## See Also

### Managing context menus

Adding context menus in your app

Provide quick access to useful actions by adding context menus to your iOS app.

func collectionView(UICollectionView, willEndContextMenuInteraction: UIContextMenuConfiguration, animator: (any UIContextMenuInteractionAnimating)?)

Informs the delegate when a context menu will disappear.

func collectionView(UICollectionView, willPerformPreviewActionForMenuWith: UIContextMenuConfiguration, animator: any UIContextMenuInteractionCommitAnimating)

Informs the delegate when a user triggers a commit by tapping the preview.

func collectionView(UICollectionView, contextMenuConfigurationForItemsAt: [IndexPath], point: CGPoint) -> UIContextMenuConfiguration?

Asks the delegate for a context-menu configuration for the items at the specified index paths.

func collectionView(UICollectionView, contextMenuConfiguration: UIContextMenuConfiguration, highlightPreviewForItemAt: IndexPath) -> UITargetedPreview?

Asks the delegate for a preview of the item at the specified index path when a context-menu interaction begins.

func collectionView(UICollectionView, contextMenuConfiguration: UIContextMenuConfiguration, dismissalPreviewForItemAt: IndexPath) -> UITargetedPreview?

Asks the delegate for a preview of the item at the specified index path when a context-menu interaction ends.

