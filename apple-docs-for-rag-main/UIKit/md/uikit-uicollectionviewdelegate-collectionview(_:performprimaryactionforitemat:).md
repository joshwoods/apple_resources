

- UIKit
- UICollectionViewDelegate
-  collectionView(\_:performPrimaryActionForItemAt:) 

Instance Method

# collectionView(\_:performPrimaryActionForItemAt:)

Tells the delegate to perform the primary action for the cell at the specified index path.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+tvOS 16.0+visionOS 1.0+

``` source
@MainActor
optional func collectionView(
    _ collectionView: UICollectionView,
    performPrimaryActionForItemAt indexPath: IndexPath
)
```

## Parameters 

`collectionView`  

The collection view object on which to perform the primary action.

`indexPath`  

The index path of the cell.

## Mentioned in 

Building a desktop-class iPad app

## Discussion

Primary actions allow you to distinguish between a distinct user action and a change in selection (like a focus change or other indirect selection change). A primary action occurs when a person selects a single cell without extending an existing selection.

UIKit calls this method after collectionView(_:shouldSelectItemAt:) and collectionView(_:didSelectItemAt:), regardless of whether the cell selection state changes. Use collectionView(_:didSelectItemAt:) to update the state of the current view controller (like its buttons, title, and so on), and use collectionView(_:performPrimaryActionForItemAt:) for actions like navigation or showing another split view column.

If collectionView(_:shouldSelectItemAt:) returns true to allow selection for the cell at `indexPath`, only that cell has selection when the system calls this method. If collectionView(_:shouldSelectItemAt:) returns false, the system preserves the existing cell selection in the collection view. You can use this behavior to perform primary actions on nonselectable, button-style cells without changing the selection.

## See Also

### Managing actions for cells

func collectionView(UICollectionView, canPerformPrimaryActionForItemAt: IndexPath) -> Bool

Asks the delegate whether to perform a primary action for the cell at the specified index path.

