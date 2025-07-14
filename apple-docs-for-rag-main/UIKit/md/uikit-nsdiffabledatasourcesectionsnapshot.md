

- UIKit
-  NSDiffableDataSourceSectionSnapshot 

Structure

# NSDiffableDataSourceSectionSnapshot

A representation of the state of the data in a layout section at a specific point in time.

iOS 14.0+iPadOS 14.0+Mac CatalysttvOS 14.0+visionOS

``` source
@preconcurrency
struct NSDiffableDataSourceSectionSnapshot where ItemIdentifierType : Hashable, ItemIdentifierType : Sendable
```

## Overview

A section snapshot represents the data for a single section in a collection view. Through a section snapshot, you set up the initial state of the data that displays in an individual section of your view, and later update that data.

You can use section snapshots with or instead of an NSDiffableDataSourceSnapshot, which represents the data in the entire view. Use a section snapshot when you need precise management of the data in a section of your layout, such as when the sections of your layout acquire their data from different sources. You can also use a section snapshot to represent data with a hierarchical structure, such as an outline with expandable items.

The following example creates a section snapshot with one root item that contains three child items:

```
for section in Section.allCases {
    // Create a section snapshot
    var sectionSnapshot = NSDiffableDataSourceSectionSnapshot()

    // Populate the section snapshot
    sectionSnapshot.append(["Food", "Drinks"])
    sectionSnapshot.append(["🍏", "🍓", "🥐"], to: "Food")

    // Apply the section snapshot
    dataSource.apply(sectionSnapshot,
                     to: section,
                     animatingDifferences: true)
}
```

## Topics

### Creating a section snapshot

init()

Creates an empty section snapshot.

init(NSDiffableDataSourceSectionSnapshot&lt;ItemIdentifierType>)

Creates a copy of the provided section snapshot.

func snapshot(of: ItemIdentifierType, includingParent: Bool) -> NSDiffableDataSourceSectionSnapshot&lt;ItemIdentifierType>

Creates a section snapshot that contains the child items of the specified parent item, optionally including the parent item.

func append([ItemIdentifierType], to: ItemIdentifierType?)

Adds the specified items as child items of the specified parent item in the section snapshot.

### Accessing items

var items: [ItemIdentifierType]

The identifiers of all items in the section snapshot.

var rootItems: [ItemIdentifierType]

The identifiers of the items at the top level of the section snapshot’s hierarchy.

var visibleItems: [ItemIdentifierType]

The identifiers of the currently visible items in the section snapshot.

### Getting item metrics

func index(of: ItemIdentifierType) -> Int?

Finds the index of the specified item in the section snapshot.

func level(of: ItemIdentifierType) -> Int

Finds the hierarchical level of the specified item in the section snapshot.

func parent(of: ItemIdentifierType) -> ItemIdentifierType?

Finds the parent item of the specified item in the section snapshot.

func contains(ItemIdentifierType) -> Bool

Indicates whether the section snapshot contains the specified item.

func isVisible(ItemIdentifierType) -> Bool

Indicates whether the specified item is currently visible onscreen.

### Inserting items

func insert([ItemIdentifierType], after: ItemIdentifierType)

Inserts the provided items immediately after the item with the specified identifier in the section snapshot.

func insert(NSDiffableDataSourceSectionSnapshot&lt;ItemIdentifierType>, after: ItemIdentifierType)

Inserts the provided section snapshot immediately after the item with the specified identifier in the section snapshot.

func insert([ItemIdentifierType], before: ItemIdentifierType)

Inserts the provided items immediately before the item with the specified identifier in the section snapshot.

func insert(NSDiffableDataSourceSectionSnapshot&lt;ItemIdentifierType>, before: ItemIdentifierType)

Inserts the provided section snapshot immediately before the item with the specified identifier in the section snapshot.

### Removing items

func delete([ItemIdentifierType])

Deletes the items with the specified identifiers, and any of their child items, from the section snapshot.

func deleteAll()

Deletes all of the items from the section snapshot.

### Replacing items

func replace(childrenOf: ItemIdentifierType, using: NSDiffableDataSourceSectionSnapshot&lt;ItemIdentifierType>)

Replaces all child items of the specified parent item with the provided section snapshot.

### Expanding and collapsing items

func isExpanded(ItemIdentifierType) -> Bool

Indicates whether the item with the specified identifier is in an expanded state.

func expand([ItemIdentifierType])

Expands the specified items in the section snapshot.

func collapse([ItemIdentifierType])

Collapses the specified items in the section snapshot.

### Debugging section snapshots

func visualDescription() -> String

Returns a string with an ASCII representation of the section snapshot.

### Supporting bridging

class NSDiffableDataSourceSectionSnapshotReference

A representation of the state of the data in a layout section at a specific point in time.

### Instance Properties

var expandedItems: [ItemIdentifierType]

## Relationships

### Conforms To

- Copyable
- Sendable

## See Also

### Data

Updating collection views using diffable data sources

Streamline the display and update of data in a collection view using a diffable data source that contains identifiers.

Implementing modern collection views

Bring compositional layouts to your app and simplify updating your user interface with diffable data sources.

Building high-performance lists and collection views

Improve the performance of lists and collections in your app with prefetching and image preparation.

class UICollectionViewDiffableDataSource

The object you use to manage data and provide cells for a collection view.

protocol UICollectionViewDataSource

The methods adopted by the object you use to manage data and provide cells for a collection view.

protocol UICollectionViewDataSourcePrefetching

A protocol that provides advance warning of the data requirements for a collection view, allowing the triggering of asynchronous data load operations.

struct NSDiffableDataSourceSnapshot

A representation of the state of the data in a view at a specific point in time.

class UIRefreshControl

A standard control that can initiate the refreshing of a scroll view’s contents.

