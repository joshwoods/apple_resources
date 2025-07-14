

- UIKit
-  NSDiffableDataSourceSectionTransaction 

Structure

# NSDiffableDataSourceSectionTransaction

A transaction that describes the changes after reordering the items in a section.

iOS 14.0+iPadOS 14.0+Mac CatalysttvOS 14.0+visionOS

``` source
@preconcurrency
struct NSDiffableDataSourceSectionTransaction where SectionIdentifierType : Hashable, SectionIdentifierType : Sendable, ItemIdentifierType : Hashable, ItemIdentifierType : Sendable
```

## Topics

### Accessing a transaction’s information

var sectionIdentifier: SectionIdentifierType

The identifier of the section for the transaction.

var initialSnapshot: NSDiffableDataSourceSectionSnapshot&lt;ItemIdentifierType>

The section snapshot before the transaction occured.

var finalSnapshot: NSDiffableDataSourceSectionSnapshot&lt;ItemIdentifierType>

The section snapshot after the transaction occured.

var difference: CollectionDifference&lt;ItemIdentifierType>

A collection of insertions and removals that describe the difference between initial and final section snapshots.

## Relationships

### Conforms To

- Sendable

## See Also

### Supporting reordering

var reorderingHandlers: UICollectionViewDiffableDataSource&lt;SectionIdentifierType, ItemIdentifierType>.ReorderingHandlers

The diffable data source’s handlers for reordering items.

struct ReorderingHandlers

Handlers for reordering items.

struct NSDiffableDataSourceTransaction

A transaction that describes the changes after reordering the items in the view.

