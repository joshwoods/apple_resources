

- AppKit
- NSCollectionView
-  reloadData() 

Instance Method

# reloadData()

Reloads all of the data for the collection view.

macOS 10.11+

``` source
@MainActor
func reloadData()
```

## Discussion

Call this method when the data in your data source object changes or when you want to force the collection view to update its contents. When you call this method, the collection view discards any currently visible items and views and redisplays them. For efficiency, the collection view displays only the items and supplementary views that are visible after reloading the data. If the collection view’s size changes as a result of reloading the data, the collection view adjusts its scrolling offsets accordingly.

Do not call this method in the middle of animation blocks where items are being inserted or deleted. The methods used to insert and delete items automatically update the collection view’s contents.

## See Also

### Reloading Content

func reloadSections(IndexSet)

Reloads the data in the specified sections of the collection view.

func reloadItems(at: Set&lt;IndexPath>)

Reloads only the specified items.

