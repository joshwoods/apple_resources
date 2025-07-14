

- UIKit
-  NSDiffableDataSourceSectionSnapshotReference 

Class

# NSDiffableDataSourceSectionSnapshotReference

A representation of the state of the data in a layout section at a specific point in time.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+tvOS 14.0+visionOS 1.0+

``` source
class NSDiffableDataSourceSectionSnapshotReference
```

## Overview

A section snapshot represents the data for a single section in a collection view. Through a section snapshot, you set up the initial state of the data that displays in an individual section of your view, and later update that data.

You can use section snapshots with or instead of an NSDiffableDataSourceSnapshotReference, which represents the data in the entire view. Use a section snapshot when you need precise management of the data in a section of your layout, such as when the sections of your layout acquire their data from different sources. You can also use a section snapshot to represent data with a hierarchical structure, such as an outline with expandable items.

The following example creates a section snapshot with one root item that contains three child items:

```
for (NSNumber *section in sections) {
    // Create a section snapshot.
    NSDiffableDataSourceSectionSnapshot *sectionSnapshot = [[NSDiffableDataSourceSectionSnapshot alloc] init];

    // Populate the section snapshot.
    [sectionSnapshot appendItems: @[@"Food", @"Drinks"]];
    [sectionSnapshot appendItems: @[@"🍏", @"🍓", @"🥐"] intoParentItem: @"Food"];

    // Apply the section snapshot.
    [dataSource applySnapshot: sectionSnapshot
                    toSection: section
         animatingDifferences: YES];
}
```

Important

If you’re working in a Swift codebase, always use NSDiffableDataSourceSectionSnapshot instead.

Avoid using this type in Swift code. Only use this type to bridge from Objective-C code to Swift code by typecasting from a section snapshot reference to a section snapshot:

```
let sectionSnapshot = sectionSnapshotRef as NSDiffableDataSourceSectionSnapshot
```

## Topics

### Creating a section snapshot

init()

Creates an empty section snapshot.

func ofParentItem(Any) -> NSDiffableDataSourceSectionSnapshotReference

Creates a section snapshot containing the child items of the specified parent item, excluding the parent item.

func ofParentItem(Any, includingParentItem: Bool) -> NSDiffableDataSourceSectionSnapshotReference

Creates a section snapshot containing the child items of the specified parent item, including the parent item.

func appendItems([Any])

Adds the specified items to the section snapshot.

func appendItems([Any], intoParentItem: Any?)

Adds the specified items as child items of the specified parent item in the section snapshot.

### Accessing items

var items: [Any]

The identifiers of all items in the section snapshot.

var rootItems: [Any]

The identifiers of the items at the top level of the section snapshot’s hierarchy.

var visibleItems: [Any]

The identifiers of the currently visible items in the section snapshot.

### Getting item metrics

func index(ofItem: Any) -> Int

Finds the index of the specified item in the section snapshot.

func level(ofItem: Any) -> Int

Finds the hierarchical level of the specified item in the section snapshot.

func parent(ofChildItem: Any) -> Any?

Finds the parent item of the specified item in the section snapshot.

func containsItem(Any) -> Bool

Indicates whether the section snapshot contains the specified item.

func isVisible(Any) -> Bool

Indicates whether the specified item is currently visible onscreen.

### Inserting items

func insert(NSDiffableDataSourceSectionSnapshotReference, afterItem: Any) -> Any

Inserts the provided section snapshot immediately after the item with the specified identifier in the section snapshot.

func insertItems([Any], afterItem: Any)

Inserts the provided items immediately after the item with the specified identifier in the section snapshot.

func insert(NSDiffableDataSourceSectionSnapshotReference, beforeItem: Any)

Inserts the provided section snapshot immediately before the item with the specified identifier in the section snapshot.

func insertItems([Any], beforeItem: Any)

Inserts the provided items immediately before the item with the specified identifier in the section snapshot.

### Removing items

func deleteItems([Any])

Deletes the items with the specified identifiers, and any of their child items, from the section snapshot.

func deleteAllItems()

Deletes all of the items from the section snapshot.

### Replacing items

func replaceChildren(ofParentItem: Any, with: NSDiffableDataSourceSectionSnapshotReference)

Replaces all child items of the specified parent item with the provided section snapshot.

### Expanding and collapsing items

func isExpanded(Any) -> Bool

Indicates whether the item with the specified identifier is in an expanded state.

func expandItems([Any])

Expands the specified items in the section snapshot.

func collapseItems([Any])

Collapses the specified items in the section snapshot.

### Debugging section snapshots

func visualDescription() -> String

Returns a string with an ASCII representation of the section snapshot.

### Instance Methods

func expandedItems() -> [Any]

The identifiers of all expanded items in the section snapshot.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCopying
- NSObjectProtocol

