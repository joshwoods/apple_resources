

- UIKit
- NSDiffableDataSourceSnapshotReference
-  insertSections(withIdentifiers:afterSectionWithIdentifier:) 

Instance Method

# insertSections(withIdentifiers:afterSectionWithIdentifier:)

Inserts the provided sections immediately after the section with the specified identifier in the snapshot.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+tvOS 13.0+visionOS 1.0+

``` source
func insertSections(
    withIdentifiers sectionIdentifiers: [Any],
    afterSectionWithIdentifier toSectionIdentifier: Any
)
```

## Parameters 

`sectionIdentifiers`  

The array of identifiers corresponding to the sections to add to the snapshot.

`toSectionIdentifier`  

The identifier of the section after which to insert the new sections.

## See Also

### Inserting items and sections

func insertItems(withIdentifiers: [Any], afterItemWithIdentifier: Any)

Inserts the provided items immediately after the item with the specified identifier in the snapshot.

func insertItems(withIdentifiers: [Any], beforeItemWithIdentifier: Any)

Inserts the provided items immediately before the item with the specified identifier in the snapshot.

func insertSections(withIdentifiers: [Any], beforeSectionWithIdentifier: Any)

Inserts the provided sections immediately before the section with the specified identifier in the snapshot.

