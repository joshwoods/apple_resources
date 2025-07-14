

- UIKit
- UICollectionViewDiffableDataSource
-  apply(\_:to:animatingDifferences:) 

Instance Method

# apply(\_:to:animatingDifferences:)

Updates the section UI to reflect the state of the data in the specified snapshot, optionally animating the UI changes.

iOS 15.0+iPadOS 15.0+Mac CatalysttvOS 15.0+visionOS

``` source
@MainActor @preconcurrency
func apply(
    _ snapshot: NSDiffableDataSourceSectionSnapshot,
    to section: SectionIdentifierType,
    animatingDifferences: Bool = true
) async
```

Available when `SectionIdentifierType` conforms to `Hashable`, `SectionIdentifierType` conforms to `Sendable`, `ItemIdentifierType` conforms to `Hashable`, and `ItemIdentifierType` conforms to `Sendable`.

## See Also

### Updating section data

func snapshot(for: SectionIdentifierType) -> NSDiffableDataSourceSectionSnapshot&lt;ItemIdentifierType>

Returns a representation of the current state of the data in the specified section of the collection view.

func apply(NSDiffableDataSourceSectionSnapshot&lt;ItemIdentifierType>, to: SectionIdentifierType, animatingDifferences: Bool, completion: (() -> Void)?)

Updates the section UI to reflect the state of the data in the specified snapshot, optionally animating the UI changes and executing a completion handler.

