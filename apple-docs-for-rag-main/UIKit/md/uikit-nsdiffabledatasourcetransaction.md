

- UIKit
-  NSDiffableDataSourceTransaction 

Structure

# NSDiffableDataSourceTransaction

A transaction that describes the changes after reordering the items in the view.

iOS 14.0+iPadOS 14.0+Mac CatalysttvOS 14.0+visionOS

``` source
@preconcurrency
struct NSDiffableDataSourceTransaction where SectionIdentifierType : Hashable, SectionIdentifierType : Sendable, ItemIdentifierType : Hashable, ItemIdentifierType : Sendable
```

## Topics

### Accessing a transaction’s information

var sectionTransactions: [NSDiffableDataSourceSectionTransaction&lt;SectionIdentifierType, ItemIdentifierType>]

An array of section transactions for the transaction.

var initialSnapshot: NSDiffableDataSourceSnapshot&lt;SectionIdentifierType, ItemIdentifierType>

The snapshot before the transaction occured.

var finalSnapshot: NSDiffableDataSourceSnapshot&lt;SectionIdentifierType, ItemIdentifierType>

The snapshot after the transaction occured.

var difference: CollectionDifference&lt;ItemIdentifierType>

A collection of insertions and removals that describe the difference between initial and final snapshots.

## Relationships

### Conforms To

- Sendable

## See Also

### Supporting reordering

var reorderingHandlers: UICollectionViewDiffableDataSource&lt;SectionIdentifierType, ItemIdentifierType>.ReorderingHandlers

The diffable data source’s handlers for reordering items.

struct ReorderingHandlers

Handlers for reordering items.

struct NSDiffableDataSourceSectionTransaction

A transaction that describes the changes after reordering the items in a section.

