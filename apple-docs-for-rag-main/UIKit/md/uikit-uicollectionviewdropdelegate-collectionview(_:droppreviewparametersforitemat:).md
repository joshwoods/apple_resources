

- UIKit
- UICollectionViewDropDelegate
-  collectionView(\_:dropPreviewParametersForItemAt:) 

Instance Method

# collectionView(\_:dropPreviewParametersForItemAt:)

Returns custom information about how to display the item at the specified location during the drop.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
optional func collectionView(
    _ collectionView: UICollectionView,
    dropPreviewParametersForItemAt indexPath: IndexPath
) -> UIDragPreviewParameters?
```

## Parameters 

`collectionView`  

The collection view that’s the destination for the drop.

`indexPath`  

The index path in the collection view to insert the item.

## Return Value

Drop parameters that indicate how to display the item during the drop.

## Discussion

Use this method to customize the appearance of the item during drops. If you don’t implement this method or if you implement it and return `nil`, the collection view uses the cell’s visible bounds to create the preview.

