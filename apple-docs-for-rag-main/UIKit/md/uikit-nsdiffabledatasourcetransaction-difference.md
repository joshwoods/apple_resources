

- UIKit
- NSDiffableDataSourceTransaction
-  difference 

Instance Property

# difference

A collection of insertions and removals that describe the difference between initial and final snapshots.

iOS 14.0+iPadOS 14.0+Mac CatalysttvOS 14.0+visionOS

``` source
var difference: CollectionDifference { get }
```

## See Also

### Accessing a transaction’s information

var sectionTransactions: [NSDiffableDataSourceSectionTransaction&lt;SectionIdentifierType, ItemIdentifierType>]

An array of section transactions for the transaction.

var initialSnapshot: NSDiffableDataSourceSnapshot&lt;SectionIdentifierType, ItemIdentifierType>

The snapshot before the transaction occured.

var finalSnapshot: NSDiffableDataSourceSnapshot&lt;SectionIdentifierType, ItemIdentifierType>

The snapshot after the transaction occured.

