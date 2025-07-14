

- UIKit
- NSDiffableDataSourceSnapshotReference
-  appendSections(withIdentifiers:) 

Instance Method

# appendSections(withIdentifiers:)

Adds the sections with the specified identifiers to the snapshot.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+tvOS 13.0+visionOS 1.0+

``` source
func appendSections(withIdentifiers sectionIdentifiers: [Any])
```

## Parameters 

`sectionIdentifiers`  

An array of identifiers specifying the sections to add to the snapshot.

## See Also

### Creating a snapshot

func appendItems(withIdentifiers: [Any], intoSectionWithIdentifier: Any)

Adds the items with the specified identifiers to the specified section of the snapshot.

func appendItems(withIdentifiers: [Any])

Adds the items with the specified identifiers to the last section of the snapshot.

