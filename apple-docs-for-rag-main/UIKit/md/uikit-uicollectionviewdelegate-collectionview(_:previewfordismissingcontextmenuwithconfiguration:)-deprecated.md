

- UIKit
- UICollectionViewDelegate
-  collectionView(\_:previewForDismissingContextMenuWithConfiguration:) Deprecated

Instance Method

# collectionView(\_:previewForDismissingContextMenuWithConfiguration:)

Returns the destination view when dismissing a context menu.

iOS 13.0–16.0DeprecatediPadOS 13.0–16.0DeprecatedMac Catalyst 13.1–16.0DeprecatedvisionOS 1.0–1.0Deprecated

``` source
@MainActor
optional func collectionView(
    _ collectionView: UICollectionView,
    previewForDismissingContextMenuWithConfiguration configuration: UIContextMenuConfiguration
) -> UITargetedPreview?
```

Deprecated

Use collectionView(_:contextMenuConfiguration:dismissalPreviewForItemAt:) instead.

## Parameters 

`collectionView`  

The collection view object requesting this information.

`configuration`  

The configuration of the menu being displayed.

## Return Value

A targeted preview object describing the dismissal preview. The interaction animates the presented menu to the preview. Use this method to customize the dismissal animation.

## See Also

### Deprecated

func collectionView(UICollectionView, targetIndexPathForMoveFromItemAt: IndexPath, toProposedIndexPath: IndexPath) -> IndexPath

Asks the delegate for the index path to use when moving an item.

Deprecated

func collectionView(UICollectionView, contextMenuConfigurationForItemAt: IndexPath, point: CGPoint) -> UIContextMenuConfiguration?

Returns a context menu configuration for the item at a point.

Deprecated

func collectionView(UICollectionView, previewForHighlightingContextMenuWithConfiguration: UIContextMenuConfiguration) -> UITargetedPreview?

Returns a view to override the default preview the collection view created.

Deprecated

func collectionView(UICollectionView, shouldShowMenuForItemAt: IndexPath) -> Bool

Asks the delegate if an action menu should be displayed for the specified item.

Deprecated

func collectionView(UICollectionView, canPerformAction: Selector, forItemAt: IndexPath, withSender: Any?) -> Bool

Asks the delegate if it can perform the specified action on an item in the collection view.

Deprecated

func collectionView(UICollectionView, performAction: Selector, forItemAt: IndexPath, withSender: Any?)

Tells the delegate to perform the specified action on an item in the collection view.

Deprecated

