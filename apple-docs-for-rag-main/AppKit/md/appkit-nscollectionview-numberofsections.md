

- AppKit
- NSCollectionView
-  numberOfSections 

Instance Property

# numberOfSections

The number of sections in the collection view.

macOS 10.11+

``` source
@MainActor
var numberOfSections: Int { get }
```

## Discussion

This property contains the number of sections reported by the data source object. If the collection view does not use a data source object, the value in this property is `1`.

## See Also

### Getting the State of the Collection View

func numberOfItems(inSection: Int) -> Int

Returns the number of items in the specified section.

