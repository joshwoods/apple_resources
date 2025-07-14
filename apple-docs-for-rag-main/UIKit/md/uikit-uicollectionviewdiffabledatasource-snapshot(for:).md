

- UIKit
- UICollectionViewDiffableDataSource
-  snapshot(for:) 

Instance Method

# snapshot(for:)

Returns a representation of the current state of the data in the specified section of the collection view.

iOS 14.0+iPadOS 14.0+Mac CatalysttvOS 14.0+visionOS

``` source
@MainActor @preconcurrency
func snapshot(for section: SectionIdentifierType) -> NSDiffableDataSourceSectionSnapshot
```

Available when `SectionIdentifierType` conforms to `Hashable`, `SectionIdentifierType` conforms to `Sendable`, `ItemIdentifierType` conforms to `Hashable`, and `ItemIdentifierType` conforms to `Sendable`.

## See Also

### Updating section data

func apply(NSDiffableDataSourceSectionSnapshot&lt;ItemIdentifierType>, to: SectionIdentifierType, animatingDifferences: Bool, completion: (() -> Void)?)

Updates the section UI to reflect the state of the data in the specified snapshot, optionally animating the UI changes and executing a completion handler.

func apply(NSDiffableDataSourceSectionSnapshot&lt;ItemIdentifierType>, to: SectionIdentifierType, animatingDifferences: Bool) async

Updates the section UI to reflect the state of the data in the specified snapshot, optionally animating the UI changes.

