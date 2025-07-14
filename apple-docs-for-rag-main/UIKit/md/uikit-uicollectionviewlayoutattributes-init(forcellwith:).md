

- UIKit
- UICollectionViewLayoutAttributes
-  init(forCellWith:) 

Initializer

# init(forCellWith:)

Creates and returns a layout attributes object that represents a cell with the specified index path.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
convenience init(forCellWith indexPath: IndexPath)
```

## Parameters 

`indexPath`  

The index path of the cell.

## Return Value

A new layout attributes object whose precise type matches the type of the class used to call this method.

## Discussion

Use this method to create a layout attributes object for a cell in the collection view. Cells are the main type of view presented by a collection view. The index path for a cell typically includes both a section index and an item index for locating the cell’s contents in the collection view’s data source.

## See Also

### Creating layout attributes

convenience init(forSupplementaryViewOfKind: String, with: IndexPath)

Creates and returns a layout attributes object that represents the specified supplementary view.

convenience init(forDecorationViewOfKind: String, with: IndexPath)

Creates and returns a layout attributes object that represents the specified decoration view.

