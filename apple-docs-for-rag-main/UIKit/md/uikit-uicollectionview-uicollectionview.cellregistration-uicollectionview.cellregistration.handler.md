

- UIKit
- UICollectionView
- UICollectionView.CellRegistration
-  UICollectionView.CellRegistration.Handler 

Type Alias

# UICollectionView.CellRegistration.Handler

A closure that handles the cell registration and configuration.

iOS 14.0+iPadOS 14.0+Mac CatalysttvOS 14.0+visionOS

``` source
typealias Handler = (Cell, IndexPath, Item) -> Void
```

## See Also

### Creating a cell registration

init(handler: UICollectionView.CellRegistration&lt;Cell, Item>.Handler)

Creates a cell registration with the specified registration handler.

init(cellNib: UINib, handler: UICollectionView.CellRegistration&lt;Cell, Item>.Handler)

Creates a cell registration with the specified registration handler and nib file.

