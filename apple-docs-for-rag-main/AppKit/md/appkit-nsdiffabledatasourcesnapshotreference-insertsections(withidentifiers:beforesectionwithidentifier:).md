

- AppKit
- NSDiffableDataSourceSnapshotReference
-  insertSections(withIdentifiers:beforeSectionWithIdentifier:) 

Instance Method

# insertSections(withIdentifiers:beforeSectionWithIdentifier:)

Inserts the provided sections immediately before the section with the specified identifier in the snapshot.

macOS 10.15+

``` source
func insertSections(
    withIdentifiers sectionIdentifiers: [Any],
    beforeSectionWithIdentifier toSectionIdentifier: Any
)
```

## Parameters 

`sectionIdentifiers`  

The array of identifiers corresponding to the sections to add to the snapshot.

`toSectionIdentifier`  

The identifier of the section before which to insert the new sections.

## See Also

### Inserting items and sections

func insertItems(withIdentifiers: [Any], afterItemWithIdentifier: Any)

Inserts the provided items immediately after the item with the specified identifier in the snapshot.

func insertItems(withIdentifiers: [Any], beforeItemWithIdentifier: Any)

Inserts the provided items immediately before the item with the specified identifier in the snapshot.

func insertSections(withIdentifiers: [Any], afterSectionWithIdentifier: Any)

Inserts the provided sections immediately after the section with the specified identifier in the snapshot.

