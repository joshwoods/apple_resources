

- UIKit
- NSDiffableDataSourceSnapshot
-  reloadItems(\_:) 

Instance Method

# reloadItems(\_:)

Reloads the data within the specified items in the snapshot.

iOS 13.0+iPadOS 13.0+Mac CatalysttvOS 13.0+visionOS

``` source
mutating func reloadItems(_ identifiers: [ItemIdentifierType])
```

## Parameters 

`identifiers`  

The array of identifiers corresponding to the items to reload in the snapshot.

## See Also

### Reloading data

func reconfigureItems([ItemIdentifierType])

Updates the data for the items you specify in the snapshot, preserving the existing cells for the items.

var reconfiguredItemIdentifiers: [ItemIdentifierType]

Identifies the items reconfigured by the changes to the snapshot.

var reloadedItemIdentifiers: [ItemIdentifierType]

Identifies the items reloaded by the changes to the snapshot.

func reloadSections([SectionIdentifierType])

Reloads the data within the specified sections of the snapshot.

var reloadedSectionIdentifiers: [SectionIdentifierType]

Identifies the sections reloaded by the changes to the snapshot.

