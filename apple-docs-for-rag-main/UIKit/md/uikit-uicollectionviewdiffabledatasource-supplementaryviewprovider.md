

- UIKit
- UICollectionViewDiffableDataSource
-  supplementaryViewProvider 

Instance Property

# supplementaryViewProvider

The closure that configures and returns the collection view’s supplementary views, such as headers and footers, from the diffable data source.

iOS 13.0+iPadOS 13.0+Mac CatalysttvOS 13.0+visionOS

``` source
@MainActor @preconcurrency
var supplementaryViewProvider: UICollectionViewDiffableDataSource.SupplementaryViewProvider? { get set }
```

## See Also

### Creating supplementary views

typealias SupplementaryViewProvider

A closure that configures and returns a collection view’s supplementary view, such as a header or footer, from a diffable data source.

