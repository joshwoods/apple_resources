

- AppKit
-  NSDiffableDataSourceSnapshot 

Structure

# NSDiffableDataSourceSnapshot

A representation of the state of the data in a view at a specific point in time.

macOS 10.15.1+

``` source
struct NSDiffableDataSourceSnapshot where SectionIdentifierType : Hashable, ItemIdentifierType : Hashable
```

## Overview

Diffable data sources use *snapshots* to provide data for collection views and table views. You use a snapshot to set up the initial state of the data that a view displays, and you use snapshots to reflect changes to the data that the view displays.

The data in a snapshot is made up of the sections and items you want to display, in the order you that you determine. You configure what to display by adding, deleting, or moving the sections and items.

Important

Each of your sections and items must have unique identifiers that conform to the Hashable protocol. Use `struct` or `enum` Swift value types for your identifiers, including built-in types such as `Int`, `String`, or `UUID`. If you use a Swift `class` for your identifiers, your `class` must be a subclass of `NSObject`.

To display data in a view using a snapshot:

1.  Create a snapshot and populate it with the state of the data you want to display.

2.  Apply the snapshot to reflect the changes in the UI.

You can create and configure a snapshot in one of these ways:

- Create an empty snapshot, then append sections and items to it.

- Get the current snapshot by calling the diffable data source’s snapshot() method, then modify that snapshot to reflect the new state of the data that you want to display.

For example, the following code creates an empty snapshot and populates it with a single section with three items. Then, the code applies the snapshot, animating the UI updates between the previous state and the new state.

```
// Create a snapshot.
var snapshot = NSDiffableDataSourceSnapshot()        

// Populate the snapshot.
snapshot.appendSections([0])
snapshot.appendItems([UUID(), UUID(), UUID()])

// Apply the snapshot.
dataSource.apply(snapshot, animatingDifferences: true)
```

For more information, see the diffable data source types:

- UICollectionViewDiffableDataSource

- UITableViewDiffableDataSource

- NSCollectionViewDiffableDataSourceReference

### Bridging

You can bridge from an NSDiffableDataSourceSnapshotReference object to this type:

```
let snapshot = snapshotReference as NSDiffableDataSourceSnapshot
```

## Topics

### Creating a Snapshot

init()

Creates an empty snapshot.

func appendSections([SectionIdentifierType])

Adds the sections with the specified identifiers to the snapshot.

func appendItems([ItemIdentifierType], toSection: SectionIdentifierType?)

Adds the items with the specified identifiers to the specified section of the snapshot.

### Getting Item and Section Metrics

var numberOfItems: Int

The number of items in the snapshot.

var numberOfSections: Int

The number of sections in the snapshot.

func numberOfItems(inSection: SectionIdentifierType) -> Int

Returns the number of items in the specified section of the snapshot.

### Identifying Items and Sections

var itemIdentifiers: [ItemIdentifierType]

The identifiers of all of the items in the snapshot.

var sectionIdentifiers: [SectionIdentifierType]

The identifiers of all of the sections in the snapshot.

func indexOfItem(ItemIdentifierType) -> Int?

Returns the index of the item in the snapshot with the specified identifier.

func indexOfSection(SectionIdentifierType) -> Int?

Returns the index of the section of the snapshot with the specified identifier.

func itemIdentifiers(inSection: SectionIdentifierType) -> [ItemIdentifierType]

Returns the identifiers of all of the items in the specified section of the snapshot.

func sectionIdentifier(containingItem: ItemIdentifierType) -> SectionIdentifierType?

Returns the identifier of the section containing the specified item in the snapshot.

### Inserting Items and Sections

func insertItems([ItemIdentifierType], afterItem: ItemIdentifierType)

Inserts the provided items immediately after the item with the specified identifier in the snapshot.

func insertItems([ItemIdentifierType], beforeItem: ItemIdentifierType)

Inserts the provided items immediately before the item with the specified identifier in the snapshot.

func insertSections([SectionIdentifierType], afterSection: SectionIdentifierType)

Inserts the provided sections immediately after the section with the specified identifier in the snapshot.

func insertSections([SectionIdentifierType], beforeSection: SectionIdentifierType)

Inserts the provided sections immediately before the section with the specified identifier in the snapshot.

### Removing Items and Sections

func deleteAllItems()

Deletes all of the items from the snapshot.

func deleteItems([ItemIdentifierType])

Deletes the items with the specified identifiers from the snapshot.

func deleteSections([SectionIdentifierType])

Deletes the sections with the specified identifiers from the snapshot.

### Reordering Items and Sections

func moveItem(ItemIdentifierType, afterItem: ItemIdentifierType)

Moves the item from its current position in the snapshot to the position immediately after the specified item.

func moveItem(ItemIdentifierType, beforeItem: ItemIdentifierType)

Moves the item from its current position in the snapshot to the position immediately before the specified item.

func moveSection(SectionIdentifierType, afterSection: SectionIdentifierType)

Moves the section from its current position in the snapshot to the position immediately after the specified section.

func moveSection(SectionIdentifierType, beforeSection: SectionIdentifierType)

Moves the section from its current position in the snapshot to the position immediately before the specified section.

### Reloading Data

func reloadItems([ItemIdentifierType])

Reloads the data within the specified items in the snapshot.

func reloadSections([SectionIdentifierType])

Reloads the data within the specified sections of the snapshot.

### Supporting Bridging

class NSDiffableDataSourceSnapshotReference

A representation of the state of the data in a view at a specific point in time.

## Relationships

### Conforms To

- Copyable

## See Also

### Data

protocol NSCollectionViewDataSource

A set of methods that a data source object implements to provide the information and view objects that a collection view requires to present content.

protocol NSCollectionViewDelegate

A set of methods that you use to manage the behavior of a collection view.

class NSCollectionViewDiffableDataSource

The object you use to manage data and provide items for a collection view.

