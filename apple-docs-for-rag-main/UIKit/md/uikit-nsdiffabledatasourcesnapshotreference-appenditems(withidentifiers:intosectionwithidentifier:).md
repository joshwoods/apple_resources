

- UIKit
- NSDiffableDataSourceSnapshotReference
-  appendItems(withIdentifiers:intoSectionWithIdentifier:) 

Instance Method

# appendItems(withIdentifiers:intoSectionWithIdentifier:)

Adds the items with the specified identifiers to the specified section of the snapshot.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+tvOS 13.0+visionOS 1.0+

``` source
func appendItems(
    withIdentifiers identifiers: [Any],
    intoSectionWithIdentifier sectionIdentifier: Any
)
```

## Parameters 

`identifiers`  

An array of identifiers specifying the items to add to the snapshot.

`sectionIdentifier`  

The section to which to add the items.

## See Also

### Creating a snapshot

func appendSections(withIdentifiers: [Any])

Adds the sections with the specified identifiers to the snapshot.

func appendItems(withIdentifiers: [Any])

Adds the items with the specified identifiers to the last section of the snapshot.

