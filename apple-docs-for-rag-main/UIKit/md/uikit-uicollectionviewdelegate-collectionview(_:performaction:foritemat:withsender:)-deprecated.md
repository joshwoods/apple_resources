

- UIKit
- UICollectionViewDelegate
-  collectionView(\_:performAction:forItemAt:withSender:) Deprecated

Instance Method

# collectionView(\_:performAction:forItemAt:withSender:)

Tells the delegate to perform the specified action on an item in the collection view.

iOS 6.0–13.0DeprecatediPadOS 6.0–13.0DeprecatedMac Catalyst 13.1–13.1DeprecatedtvOSDeprecated

``` source
@MainActor
optional func collectionView(
    _ collectionView: UICollectionView,
    performAction action: Selector,
    forItemAt indexPath: IndexPath,
    withSender sender: Any?
)
```

## Parameters 

`collectionView`  

The collection view object that is making the request.

`action`  

The selector representing the action to be performed.

`indexPath`  

The index path of the affected item.

`sender`  

The object that initiated the action.

## Discussion

If the user taps an action in the editing menu, the collection view calls this method. Your implementation of this method should do whatever is appropriate for the action. For example, for a copy action, it should extract the relevant item content and write it to the general pasteboard or an application (private) pasteboard.

For information about how to perform pasteboard-related operations, see UIPasteboard.

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

func collectionView(UICollectionView, shouldShowMenuForItemAt: IndexPath) -> Bool

Asks the delegate if an action menu should be displayed for the specified item.

Deprecated

func collectionView(UICollectionView, canPerformAction: Selector, forItemAt: IndexPath, withSender: Any?) -> Bool

Asks the delegate if it can perform the specified action on an item in the collection view.

Deprecated

