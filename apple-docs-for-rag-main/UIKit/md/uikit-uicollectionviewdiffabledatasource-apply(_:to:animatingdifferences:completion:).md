

- UIKit
- UICollectionViewDiffableDataSource
-  apply(\_:to:animatingDifferences:completion:) 

Instance Method

# apply(\_:to:animatingDifferences:completion:)

Updates the section UI to reflect the state of the data in the specified snapshot, optionally animating the UI changes and executing a completion handler.

iOS 14.0+iPadOS 14.0+Mac CatalysttvOS 14.0+visionOS

``` source
@MainActor @preconcurrency
func apply(
    _ snapshot: NSDiffableDataSourceSectionSnapshot,
    to section: SectionIdentifierType,
    animatingDifferences: Bool = true,
    completion: (() -> Void)? = nil
)
```

Available when `SectionIdentifierType` conforms to `Hashable`, `SectionIdentifierType` conforms to `Sendable`, `ItemIdentifierType` conforms to `Hashable`, and `ItemIdentifierType` conforms to `Sendable`.

## See Also

### Updating section data

func snapshot(for: SectionIdentifierType) -> NSDiffableDataSourceSectionSnapshot&lt;ItemIdentifierType>

Returns a representation of the current state of the data in the specified section of the collection view.

func apply(NSDiffableDataSourceSectionSnapshot&lt;ItemIdentifierType>, to: SectionIdentifierType, animatingDifferences: Bool) async

Updates the section UI to reflect the state of the data in the specified snapshot, optionally animating the UI changes.

