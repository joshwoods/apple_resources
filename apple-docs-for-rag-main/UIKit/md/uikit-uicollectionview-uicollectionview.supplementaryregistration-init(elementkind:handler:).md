

- UIKit
- UICollectionView
- UICollectionView.SupplementaryRegistration
-  init(elementKind:handler:) 

Initializer

# init(elementKind:handler:)

Creates a supplementary registration for the specified element kind with a registration handler.

iOS 14.0+iPadOS 14.0+Mac CatalysttvOS 14.0+visionOS

``` source
init(
    elementKind: String,
    handler: @escaping UICollectionView.SupplementaryRegistration.Handler
)
```

## See Also

### Creating a supplementary registration

init(supplementaryNib: UINib, elementKind: String, handler: UICollectionView.SupplementaryRegistration&lt;Supplementary>.Handler)

Creates a supplementary registration for the specified element kind with a registration handler and nib file.

typealias Handler

A closure that handles the supplementary view registration and configuration.

