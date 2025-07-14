

- UIKit
- NSDiffableDataSourceSectionTransaction
-  initialSnapshot 

Instance Property

# initialSnapshot

The section snapshot before the transaction occured.

iOS 14.0+iPadOS 14.0+Mac CatalysttvOS 14.0+visionOS

``` source
var initialSnapshot: NSDiffableDataSourceSectionSnapshot { get }
```

## See Also

### Accessing a transaction’s information

var sectionIdentifier: SectionIdentifierType

The identifier of the section for the transaction.

var finalSnapshot: NSDiffableDataSourceSectionSnapshot&lt;ItemIdentifierType>

The section snapshot after the transaction occured.

var difference: CollectionDifference&lt;ItemIdentifierType>

A collection of insertions and removals that describe the difference between initial and final section snapshots.

