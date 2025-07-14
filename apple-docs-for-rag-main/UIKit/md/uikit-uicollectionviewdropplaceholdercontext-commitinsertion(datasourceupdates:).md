

- UIKit
- UICollectionViewDropPlaceholderContext
-  commitInsertion(dataSourceUpdates:) 

Instance Method

# commitInsertion(dataSourceUpdates:)

Exchanges the placeholder cell for a cell with the final content.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
func commitInsertion(dataSourceUpdates: (IndexPath) -> Void) -> Bool
```

**Required**

## Parameters 

`dataSourceUpdates`  

The handler block to execute as part of committing your changes. Use this block to update your collection view’s data source with the actual data that you received. This block has no return value and takes the following parameter:

insertionIndexPath  
The location at which to insert any items. Always use this index path for the insertion point instead of any cached values.

## Return Value

true if the placeholder was replaced by your content or false if the placeholder was no longer in the collection view.

## Mentioned in 

Supporting Drag and Drop in Collection Views

## Discussion

When you receive the actual data for a cell, call this method to remove the corresponding placeholder cell and insert the actual cell. If the placeholder cell is still present in the collection view, this method calls the `dataSourceUpdates` handler. Use that handler block to update the data source object of the collection view. Do not update the collection view itself. This method automatically updates the collection view, creating a new cell for your data.

If the placeholder cell is no longer present, this method does not execute your `dataSourceUpdates` block.

## See Also

### Updating the Placeholder Cell

func setNeedsCellUpdate()

Updates the contents of the placeholder cell.

**Required**

