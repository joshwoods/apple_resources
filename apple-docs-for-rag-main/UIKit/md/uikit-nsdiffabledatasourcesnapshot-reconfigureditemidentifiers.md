

- UIKit
- NSDiffableDataSourceSnapshot
-  reconfiguredItemIdentifiers 

Instance Property

# reconfiguredItemIdentifiers

Identifies the items reconfigured by the changes to the snapshot.

iOS 15.0+iPadOS 15.0+Mac CatalysttvOS 15.0+visionOS

``` source
var reconfiguredItemIdentifiers: [ItemIdentifierType] { get }
```

## Discussion

After you make updates to the snapshot, this method returns an array of identifiers corresponding to the items that the view reconfigures when you apply the snapshot to your data source.

## See Also

### Reloading data

func reconfigureItems([ItemIdentifierType])

Updates the data for the items you specify in the snapshot, preserving the existing cells for the items.

func reloadItems([ItemIdentifierType])

Reloads the data within the specified items in the snapshot.

var reloadedItemIdentifiers: [ItemIdentifierType]

Identifies the items reloaded by the changes to the snapshot.

func reloadSections([SectionIdentifierType])

Reloads the data within the specified sections of the snapshot.

var reloadedSectionIdentifiers: [SectionIdentifierType]

Identifies the sections reloaded by the changes to the snapshot.

