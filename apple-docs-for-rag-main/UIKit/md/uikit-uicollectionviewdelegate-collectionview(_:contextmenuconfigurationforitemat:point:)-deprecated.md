

- UIKit
- UICollectionViewDelegate
-  collectionView(\_:contextMenuConfigurationForItemAt:point:) Deprecated

Instance Method

# collectionView(\_:contextMenuConfigurationForItemAt:point:)

Returns a context menu configuration for the item at a point.

iOS 13.0–16.0DeprecatediPadOS 13.0–16.0DeprecatedMac Catalyst 13.1–16.0DeprecatedvisionOS 1.0–1.0Deprecated

``` source
@MainActor
optional func collectionView(
    _ collectionView: UICollectionView,
    contextMenuConfigurationForItemAt indexPath: IndexPath,
    point: CGPoint
) -> UIContextMenuConfiguration?
```

Deprecated

Use collectionView(_:contextMenuConfigurationForItemsAt:point:) instead.

## Parameters 

`collectionView`  

The collection view containing the item.

`indexPath`  

The index path of the item for which a configuration is being requested.

`point`  

The location of the interaction in the collection view’s coordinate space.

## Return Value

A contextual menu configuration object describing the menu to be presented. Returning `nil` prevents the interaction from beginning. Returning an empty configuration object causes the interaction to begin, and then end with a cancellation effect.

## Discussion

You can use the cancellation effect from returning an empty configuration to indicate to users that it’s possible for a menu to be presented from this item, but that there are no actions to present at this particular time.

## See Also

### Deprecated

func collectionView(UICollectionView, targetIndexPathForMoveFromItemAt: IndexPath, toProposedIndexPath: IndexPath) -> IndexPath

Asks the delegate for the index path to use when moving an item.

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

