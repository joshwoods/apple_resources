

- UIKit
- NSDiffableDataSourceSnapshotReference
-  appendItems(withIdentifiers:) 

Instance Method

# appendItems(withIdentifiers:)

Adds the items with the specified identifiers to the last section of the snapshot.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+tvOS 13.0+visionOS 1.0+

``` source
func appendItems(withIdentifiers identifiers: [Any])
```

## Parameters 

`identifiers`  

An array of identifiers specifying the items to add to the snapshot.

## See Also

### Creating a snapshot

func appendSections(withIdentifiers: [Any])

Adds the sections with the specified identifiers to the snapshot.

func appendItems(withIdentifiers: [Any], intoSectionWithIdentifier: Any)

Adds the items with the specified identifiers to the specified section of the snapshot.

