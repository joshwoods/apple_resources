

- UIKit
- NSDiffableDataSourceSnapshotReference
-  reloadItems(withIdentifiers:) 

Instance Method

# reloadItems(withIdentifiers:)

Reloads the data within the specified items in the snapshot.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+tvOS 13.0+visionOS 1.0+

``` source
func reloadItems(withIdentifiers identifiers: [Any])
```

## Parameters 

`identifiers`  

The array of identifiers corresponding to the items to reload in the snapshot.

## See Also

### Reloading data

func reconfigureItems(withIdentifiers: [Any])

Updates the data for the items you specify in the snapshot, preserving the existing cells for the items.

var reconfiguredItemIdentifiers: [Any]

Identifies the items reconfigured by the changes to the snapshot.

var reloadedItemIdentifiers: [Any]

Identifies the items reloaded by the changes to the snapshot.

func reloadSections(withIdentifiers: [Any])

Reloads the data within the specified sections of the snapshot.

var reloadedSectionIdentifiers: [Any]

Identifies the sections reloaded by the changes to the snapshot.

