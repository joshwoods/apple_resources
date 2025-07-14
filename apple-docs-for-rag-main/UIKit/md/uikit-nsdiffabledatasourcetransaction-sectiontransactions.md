

- UIKit
- NSDiffableDataSourceTransaction
-  sectionTransactions 

Instance Property

# sectionTransactions

An array of section transactions for the transaction.

iOS 14.0+iPadOS 14.0+Mac CatalysttvOS 14.0+visionOS

``` source
var sectionTransactions: [NSDiffableDataSourceSectionTransaction] { get }
```

## See Also

### Accessing a transaction’s information

var initialSnapshot: NSDiffableDataSourceSnapshot&lt;SectionIdentifierType, ItemIdentifierType>

The snapshot before the transaction occured.

var finalSnapshot: NSDiffableDataSourceSnapshot&lt;SectionIdentifierType, ItemIdentifierType>

The snapshot after the transaction occured.

var difference: CollectionDifference&lt;ItemIdentifierType>

A collection of insertions and removals that describe the difference between initial and final snapshots.

