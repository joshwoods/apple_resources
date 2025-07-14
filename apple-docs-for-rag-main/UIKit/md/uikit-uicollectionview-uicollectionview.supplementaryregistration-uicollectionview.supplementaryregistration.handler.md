

- UIKit
- UICollectionView
- UICollectionView.SupplementaryRegistration
-  UICollectionView.SupplementaryRegistration.Handler 

Type Alias

# UICollectionView.SupplementaryRegistration.Handler

A closure that handles the supplementary view registration and configuration.

iOS 14.0+iPadOS 14.0+Mac CatalysttvOS 14.0+visionOS

``` source
typealias Handler = (Supplementary, String, IndexPath) -> Void
```

## See Also

### Creating a supplementary registration

init(elementKind: String, handler: UICollectionView.SupplementaryRegistration&lt;Supplementary>.Handler)

Creates a supplementary registration for the specified element kind with a registration handler.

init(supplementaryNib: UINib, elementKind: String, handler: UICollectionView.SupplementaryRegistration&lt;Supplementary>.Handler)

Creates a supplementary registration for the specified element kind with a registration handler and nib file.

