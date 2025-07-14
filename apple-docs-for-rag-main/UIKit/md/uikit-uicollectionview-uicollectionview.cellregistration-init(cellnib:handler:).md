

- UIKit
- UICollectionView
- UICollectionView.CellRegistration
-  init(cellNib:handler:) 

Initializer

# init(cellNib:handler:)

Creates a cell registration with the specified registration handler and nib file.

iOS 14.0+iPadOS 14.0+Mac CatalysttvOS 14.0+visionOS 1.0–1.0Deprecated

``` source
init(
    cellNib: UINib,
    handler: @escaping UICollectionView.CellRegistration.Handler
)
```

## See Also

### Creating a cell registration

init(handler: UICollectionView.CellRegistration&lt;Cell, Item>.Handler)

Creates a cell registration with the specified registration handler.

typealias Handler

A closure that handles the cell registration and configuration.

