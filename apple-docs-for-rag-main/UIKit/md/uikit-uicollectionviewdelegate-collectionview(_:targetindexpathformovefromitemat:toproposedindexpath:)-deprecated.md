

- UIKit
- UICollectionViewDelegate
-  collectionView(\_:targetIndexPathForMoveFromItemAt:toProposedIndexPath:) Deprecated

Instance Method

# collectionView(\_:targetIndexPathForMoveFromItemAt:toProposedIndexPath:)

Asks the delegate for the index path to use when moving an item.

iOS 9.0–15.0DeprecatediPadOS 9.0–15.0DeprecatedMac Catalyst 13.1–15.0DeprecatedtvOS 9.0–15.0DeprecatedvisionOS 1.0–1.0Deprecated

``` source
@MainActor
optional func collectionView(
    _ collectionView: UICollectionView,
    targetIndexPathForMoveFromItemAt currentIndexPath: IndexPath,
    toProposedIndexPath proposedIndexPath: IndexPath
) -> IndexPath
```

Deprecated

Use collectionView(_:targetIndexPathForMoveOfItemFromOriginalIndexPath:atCurrentIndexPath:toProposedIndexPath:) instead.

## Parameters 

`collectionView`  

The collection view making the request.

`currentIndexPath`  

The item’s original index path.

`proposedIndexPath`  

The proposed index path of the item.

## Return Value

The index path you want to use for the item. If you do not implement this method, the collection view uses the index path in the `proposedIndexPath` parameter.

## Discussion

During the interactive moving of an item, the collection view calls this method to see if you want to provide a different index path than the proposed path. You might use this method to prevent the user from dropping the item in an invalid location. For example, you might prevent the user from dropping the item in a specific section.

## See Also

### Deprecated

func collectionView(UICollectionView, contextMenuConfigurationForItemAt: IndexPath, point: CGPoint) -> UIContextMenuConfiguration?

Returns a context menu configuration for the item at a point.

Deprecated

func collectionView(UICollectionView, previewForDismissingContextMenuWithConfiguration: UIContextMenuConfiguration) -> UITargetedPreview?

Returns the destination view when dismissing a context menu.

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

