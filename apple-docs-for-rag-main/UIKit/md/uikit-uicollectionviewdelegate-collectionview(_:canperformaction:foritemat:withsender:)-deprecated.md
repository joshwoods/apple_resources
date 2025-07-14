

- UIKit
- UICollectionViewDelegate
-  collectionView(\_:canPerformAction:forItemAt:withSender:) Deprecated

Instance Method

# collectionView(\_:canPerformAction:forItemAt:withSender:)

Asks the delegate if it can perform the specified action on an item in the collection view.

iOS 6.0–13.0DeprecatediPadOS 6.0–13.0DeprecatedMac Catalyst 13.1–13.1DeprecatedtvOSDeprecated

``` source
@MainActor
optional func collectionView(
    _ collectionView: UICollectionView,
    canPerformAction action: Selector,
    forItemAt indexPath: IndexPath,
    withSender sender: Any?
) -> Bool
```

## Parameters 

`collectionView`  

The collection view object that is making the request.

`action`  

The selector identifying the action to be performed.

`indexPath`  

The index path of the affected item.

`sender`  

The object that wants to initiate the action.

## Return Value

true if the command corresponding to action should appear in the editing menu or false if it should not.

## Discussion

This method is invoked after the collectionView(_:shouldShowMenuForItemAt:) method. It gives you the opportunity to exclude commands from the editing menu. For example, the user might have copied some content from one item and wants to paste it into another item that cannot accept the content. In such a case, your method could return false to prevent the display of the relevant command.

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

func collectionView(UICollectionView, shouldShowMenuForItemAt: IndexPath) -> Bool

Asks the delegate if an action menu should be displayed for the specified item.

Deprecated

func collectionView(UICollectionView, performAction: Selector, forItemAt: IndexPath, withSender: Any?)

Tells the delegate to perform the specified action on an item in the collection view.

Deprecated

