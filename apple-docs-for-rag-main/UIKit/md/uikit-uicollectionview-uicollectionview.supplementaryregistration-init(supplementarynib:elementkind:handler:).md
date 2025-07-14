

- UIKit
- UICollectionView
- UICollectionView.SupplementaryRegistration
-  init(supplementaryNib:elementKind:handler:) 

Initializer

# init(supplementaryNib:elementKind:handler:)

Creates a supplementary registration for the specified element kind with a registration handler and nib file.

iOS 14.0+iPadOS 14.0+Mac CatalysttvOS 14.0+visionOS 1.0–1.0Deprecated

``` source
init(
    supplementaryNib: UINib,
    elementKind: String,
    handler: @escaping UICollectionView.SupplementaryRegistration.Handler
)
```

## See Also

### Creating a supplementary registration

init(elementKind: String, handler: UICollectionView.SupplementaryRegistration&lt;Supplementary>.Handler)

Creates a supplementary registration for the specified element kind with a registration handler.

typealias Handler

A closure that handles the supplementary view registration and configuration.

