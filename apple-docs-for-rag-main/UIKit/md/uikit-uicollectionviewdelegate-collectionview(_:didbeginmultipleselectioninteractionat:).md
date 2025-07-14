

- UIKit
- UICollectionViewDelegate
-  collectionView(\_:didBeginMultipleSelectionInteractionAt:) 

Instance Method

# collectionView(\_:didBeginMultipleSelectionInteractionAt:)

Tells the delegate when the user starts using a two-finger pan gesture to select multiple items in a collection view.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
optional func collectionView(
    _ collectionView: UICollectionView,
    didBeginMultipleSelectionInteractionAt indexPath: IndexPath
)
```

## Parameters 

`collectionView`  

The collection view calling this method.

`indexPath`  

The index path of the item that the user touched to start the two-finger pan gesture.

## Discussion

Your implementation of this method is a good place to indicate, in the app’s user interface, that the user is selecting multiple items; for example, you could replace an Edit or Select button with a Done button.

```
func collectionView(_ collectionView: UICollectionView, didBeginMultipleSelectionInteractionAt indexPath: IndexPath) {
    // Replace the Select button with Done, and put the 
    // collection view into editing mode.
    setEditing(true, animated: true)
}
```

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

func collectionViewDidEndMultipleSelectionInteraction(UICollectionView)

Tells the delegate when the user stops using a two-finger pan gesture to select multiple items in a collection view.

