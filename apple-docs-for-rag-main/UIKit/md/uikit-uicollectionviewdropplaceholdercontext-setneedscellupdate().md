

- UIKit
- UICollectionViewDropPlaceholderContext
-  setNeedsCellUpdate() 

Instance Method

# setNeedsCellUpdate()

Updates the contents of the placeholder cell.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
func setNeedsCellUpdate()
```

**Required**

## Discussion

Call this method when you want to update the contents of the placeholder cell. When you call this method, UIKit calls the update handler that you originally passed to the `drop(_:toPlaceholderInsertedAt:withReuseIdentifier:cellUpdateHandler:)` method when creating the cell.

## See Also

### Updating the Placeholder Cell

func commitInsertion(dataSourceUpdates: (IndexPath) -> Void) -> Bool

Exchanges the placeholder cell for a cell with the final content.

**Required**

