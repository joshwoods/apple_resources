

- UIKit
- UICollectionViewDelegate
-  collectionView(\_:shouldShowMenuForItemAt:) Deprecated

Instance Method

# collectionView(\_:shouldShowMenuForItemAt:)

Asks the delegate if an action menu should be displayed for the specified item.

iOS 6.0–13.0DeprecatediPadOS 6.0–13.0DeprecatedMac Catalyst 13.1–13.1DeprecatedtvOSDeprecated

``` source
@MainActor
optional func collectionView(
    _ collectionView: UICollectionView,
    shouldShowMenuForItemAt indexPath: IndexPath
) -> Bool
```

## Parameters 

`collectionView`  

The collection view object that is making the request.

`indexPath`  

The index path of the affected item.

## Return Value

true if the editing menu should be shown positioned near the item and pointing to it or false if it should not.

## Discussion

If the user tap-holds a certain item in the collection view, this method (if implemented) is invoked first. Return true if you want to permit the editing menu to be displayed. Return false if the editing menu shouldn’t be shown—for example, you might return false if the corresponding item contains data that should not be copied or pasted over.

If you do not implement this method, the default return value is false.

## See Also

### Deprecated

func collectionView(UICollectionView, targetIndexPathForMoveFromItemAt: IndexPath, toProposedIndexPath: IndexPath) -> IndexPath

Asks the delegate for the index path to use when moving an item.

Deprecated

func collectionView(UICollectionView, contextMenuConfigurationForItemAt: IndexPath, point: CGPoint) -> UIContextMenuConfiguration?

Returns a context menu configuration for the item at a point.

Deprecated

func collectionView(UICollectionView, previewForDismissingContextMenuWithConfiguration: UIContextMenuConfiguration) -> UITargetedPreview?

Returns the destination view when dismissing a context menu.

Deprecated

func collectionView(UICollectionView, previewForHighlightingContextMenuWithConfiguration: UIContextMenuConfiguration) -> UITargetedPreview?

Returns a view to override the default preview the collection view created.

Deprecated

func collectionView(UICollectionView, canPerformAction: Selector, forItemAt: IndexPath, withSender: Any?) -> Bool

Asks the delegate if it can perform the specified action on an item in the collection view.

Deprecated

func collectionView(UICollectionView, performAction: Selector, forItemAt: IndexPath, withSender: Any?)

Tells the delegate to perform the specified action on an item in the collection view.

Deprecated

