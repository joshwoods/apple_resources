

- UIKit
- UICollectionViewDelegate
-  collectionView(\_:shouldBeginMultipleSelectionInteractionAt:) 

Instance Method

# collectionView(\_:shouldBeginMultipleSelectionInteractionAt:)

Asks the delegate whether the user can select multiple items using a two-finger pan gesture in a collection view.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
optional func collectionView(
    _ collectionView: UICollectionView,
    shouldBeginMultipleSelectionInteractionAt indexPath: IndexPath
) -> Bool
```

## Parameters 

`collectionView`  

The collection view calling this method.

`indexPath`  

The index path of the item that the user touched to start the two-finger pan gesture.

## Return Value

true to allow the user to select multiple items using a two-finger pan gesture; otherwise, false to disable the behavior. The default value is false.

## Discussion

When the system recognizes a two-finger pan gesture, it calls this method before it sets isEditing to true. If you return true from this method, the user can select multiple items using a two-finger pan gesture.

Users can select multiple items using the two-finger pan gesture on collection views that scroll either horizontally or vertically, but not both. Collection views that scroll in both directions won’t recognize the gesture or call this method.

If you don’t implement this method, the system uses the value of allowsMultipleSelectionDuringEditing to determine whether a user can select multiple items using a pan gesture.

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

func collectionView(UICollectionView, didBeginMultipleSelectionInteractionAt: IndexPath)

Tells the delegate when the user starts using a two-finger pan gesture to select multiple items in a collection view.

func collectionViewDidEndMultipleSelectionInteraction(UICollectionView)

Tells the delegate when the user stops using a two-finger pan gesture to select multiple items in a collection view.

