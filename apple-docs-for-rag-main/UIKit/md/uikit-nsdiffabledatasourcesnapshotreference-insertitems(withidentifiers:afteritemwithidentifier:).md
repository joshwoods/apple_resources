

- UIKit
- NSDiffableDataSourceSnapshotReference
-  insertItems(withIdentifiers:afterItemWithIdentifier:) 

Instance Method

# insertItems(withIdentifiers:afterItemWithIdentifier:)

Inserts the provided items immediately after the item with the specified identifier in the snapshot.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+tvOS 13.0+visionOS 1.0+

``` source
func insertItems(
    withIdentifiers identifiers: [Any],
    afterItemWithIdentifier itemIdentifier: Any
)
```

## Parameters 

`identifiers`  

The array of identifiers corresponding to the items to add to the snapshot.

`itemIdentifier`  

The identifier of the item after which to insert the new items.

## See Also

### Inserting items and sections

func insertItems(withIdentifiers: [Any], beforeItemWithIdentifier: Any)

Inserts the provided items immediately before the item with the specified identifier in the snapshot.

func insertSections(withIdentifiers: [Any], afterSectionWithIdentifier: Any)

Inserts the provided sections immediately after the section with the specified identifier in the snapshot.

func insertSections(withIdentifiers: [Any], beforeSectionWithIdentifier: Any)

Inserts the provided sections immediately before the section with the specified identifier in the snapshot.

