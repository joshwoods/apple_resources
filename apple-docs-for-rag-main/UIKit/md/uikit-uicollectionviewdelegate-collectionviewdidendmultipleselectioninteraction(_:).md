

- UIKit
- UICollectionViewDelegate
-  collectionViewDidEndMultipleSelectionInteraction(\_:) 

Instance Method

# collectionViewDidEndMultipleSelectionInteraction(\_:)

Tells the delegate when the user stops using a two-finger pan gesture to select multiple items in a collection view.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
optional func collectionViewDidEndMultipleSelectionInteraction(_ collectionView: UICollectionView)
```

## Parameters 

`collectionView`  

The collection view calling this method.

## Discussion

The collection view calls this method after the user lifts their finger from the device.

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

func collectionView(UICollectionView, didDeselectItemAt: IndexPath)

Tells the delegate that the item at the specified path was deselected.

func collectionView(UICollectionView, shouldBeginMultipleSelectionInteractionAt: IndexPath) -> Bool

Asks the delegate whether the user can select multiple items using a two-finger pan gesture in a collection view.

func collectionView(UICollectionView, didBeginMultipleSelectionInteractionAt: IndexPath)

Tells the delegate when the user starts using a two-finger pan gesture to select multiple items in a collection view.

