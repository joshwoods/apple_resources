

- AppKit
- NSCollectionViewDiffableDataSource
-  supplementaryViewProvider 

Instance Property

# supplementaryViewProvider

The closure that configures and returns the collection view’s supplementary views, such as headers and footers, from the diffable data source.

macOS 10.15.1+

``` source
var supplementaryViewProvider: NSCollectionViewDiffableDataSource.SupplementaryViewProvider? { get set }
```

## See Also

### Creating Supplementary Views

typealias SupplementaryViewProvider

A closure that configures and returns a collection view’s supplementary view, such as a header or footer, from a diffable data source.

