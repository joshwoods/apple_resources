

- UIKit
- NSDiffableDataSourceSectionTransaction
-  sectionIdentifier 

Instance Property

# sectionIdentifier

The identifier of the section for the transaction.

iOS 14.0+iPadOS 14.0+Mac CatalysttvOS 14.0+visionOS

``` source
var sectionIdentifier: SectionIdentifierType { get }
```

## See Also

### Accessing a transaction’s information

var initialSnapshot: NSDiffableDataSourceSectionSnapshot&lt;ItemIdentifierType>

The section snapshot before the transaction occured.

var finalSnapshot: NSDiffableDataSourceSectionSnapshot&lt;ItemIdentifierType>

The section snapshot after the transaction occured.

var difference: CollectionDifference&lt;ItemIdentifierType>

A collection of insertions and removals that describe the difference between initial and final section snapshots.

