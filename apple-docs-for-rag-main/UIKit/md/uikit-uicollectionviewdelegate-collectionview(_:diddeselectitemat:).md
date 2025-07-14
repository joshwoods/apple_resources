

- UIKit
- UICollectionViewDelegate
-  collectionView(\_:didDeselectItemAt:) 

Instance Method

# collectionView(\_:didDeselectItemAt:)

Tells the delegate that the item at the specified path was deselected.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+tvOS 9.0+visionOS 1.0+

``` source
@MainActor
optional func collectionView(
    _ collectionView: UICollectionView,
    didDeselectItemAt indexPath: IndexPath
)
```

## Parameters 

`collectionView`  

The collection view object that is notifying you of the selection change.

`indexPath`  

The index path of the cell that was deselected.

## Discussion

The collection view calls this method when the user successfully deselects an item in the collection view. It does not call this method when you programmatically deselect items.

## See Also

### Managing the selected cells

Changing the appearance of selected and highlighted cells

Provide visual feedback to the user about the state of a cell and the transition between states.

Selecting multiple items with a two-finger pan gesture

Accelerate user selection of multiple items using the multiselect gesture on table and collection views.

func collectionView(UICollectionView, shouldSelectItemAt: IndexPath) -> Bool

Asks the delegate if the specified item should be selected.

func collectionView(UICollectionView, didSelectItemAt: IndexPath)

Tells the delegate that the item at the specified index path was selected.

func collectionView(UICollectionView, shouldDeselectItemAt: IndexPath) -> Bool

Asks the delegate if the specified item should be deselected.

func collectionView(UICollectionView, shouldBeginMultipleSelectionInteractionAt: IndexPath) -> Bool

Asks the delegate whether the user can select multiple items using a two-finger pan gesture in a collection view.

func collectionView(UICollectionView, didBeginMultipleSelectionInteractionAt: IndexPath)

Tells the delegate when the user starts using a two-finger pan gesture to select multiple items in a collection view.

func collectionViewDidEndMultipleSelectionInteraction(UICollectionView)

Tells the delegate when the user stops using a two-finger pan gesture to select multiple items in a collection view.

