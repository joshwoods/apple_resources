

- UIKit
- UICollectionView
- UICollectionView.CellRegistration
-  init(handler:) 

Initializer

# init(handler:)

Creates a cell registration with the specified registration handler.

iOS 14.0+iPadOS 14.0+Mac CatalysttvOS 14.0+visionOS

``` source
init(handler: @escaping UICollectionView.CellRegistration.Handler)
```

## See Also

### Creating a cell registration

init(cellNib: UINib, handler: UICollectionView.CellRegistration&lt;Cell, Item>.Handler)

Creates a cell registration with the specified registration handler and nib file.

typealias Handler

A closure that handles the cell registration and configuration.

