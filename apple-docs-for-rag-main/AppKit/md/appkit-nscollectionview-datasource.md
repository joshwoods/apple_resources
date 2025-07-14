

- AppKit
- NSCollectionView
-  dataSource 

Instance Property

# dataSource

An object that provides data for the collection view.

macOS 10.11+

``` source
@MainActor
weak var dataSource: (any NSCollectionViewDataSource)? { get set }
```

## Discussion

The data source object manages the data in the collection view. Use this object to specify how many items are in the collection view and to create the visual representation of those items. The object you specify must adopt the NSCollectionViewDataSource protocol.

To specify the data for your collection view, assign a value to this property or to the content property, but not both. If you specify a value for this property, the collection view ignores the content property and the `content` binding.

## See Also

### Providing the Collection View’s Data

protocol NSCollectionViewDataSource

A set of methods that a data source object implements to provide the information and view objects that a collection view requires to present content.

