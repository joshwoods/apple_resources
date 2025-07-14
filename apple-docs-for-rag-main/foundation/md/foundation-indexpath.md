

- Foundation
-  IndexPath 

Structure

# IndexPath

A list of indexes that together represent the path to a specific location in a tree of nested arrays.

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
struct IndexPath
```

## Overview

Each index in an index path represents the index into an array of children from one node in the tree to another, deeper, node.

## Topics

### Creating Index Paths

init()

Creates an empty index path.

init(index: IndexPath.Element)

Creates an index path with a single element.

init(arrayLiteral: IndexPath.Element...)

Creates an index path from an array literal.

init(indexes: Array&lt;IndexPath.Element>)

Creates an index path from an array of elements.

init&lt;ElementSequence>(indexes: ElementSequence)

Creates an index path from a sequence of integers.

### Working with Special Node Names

UIKit and AppKit supply specialized names for the first two index path nodes for use when working with table views and collection views.

var item: Int

The value of the item element of the index path.

var row: Int

The value of the row element of the index path.

var section: Int

The value of the section element of the index path.

### Adding Nodes

static func + (IndexPath, IndexPath) -> IndexPath

Combines the elements of two index paths into a single index path.

static func += (inout IndexPath, IndexPath)

Appends the elements of another index path to this index path.

### Selecting Nodes

func append(IndexPath)

Appends the nodes of another index path to this one.

func append(Array&lt;IndexPath.Element>)

Appends an array of elements to this index path as additional nodes.

func append(IndexPath.Element)

Appends a single element to this index path as a new node.

func appending(IndexPath.Element) -> IndexPath

Returns a new index path containing the elements of this one plus the given element.

func appending(IndexPath) -> IndexPath

Returns a new index path containing the elements of this one plus those of another index path.

func appending(Array&lt;IndexPath.Element>) -> IndexPath

Returns a new index path containing the elements of this one plus an array of additional elements.

func compare(IndexPath) -> ComparisonResult

Compares this index path to another in depth-first traversal order.

func dropLast() -> IndexPath

Return a new index path containing all but the last element.

### Excluding Nodes

func dropLast() -> IndexPath

Return a new index path containing all but the last element.

### Comparing Index Paths

func compare(IndexPath) -> ComparisonResult

Compares this index path to another in depth-first traversal order.

### Using Reference Types

class NSIndexPath

A list of indexes that together represent the path to a specific location in a tree of nested arrays.

### Initializers

init(item: Int, section: Int)

Creates an index path that references an item in a particular section.

init(item: Int, section: Int)

Initialize for use with `NSCollectionView`.

init(row: Int, section: Int)

Creates an index path that references a row in a particular section.

### Instance Properties

var item: Int

The item of this index path, when used with `NSCollectionView`.

var section: Int

The section of this index path, when used with `NSCollectionView`.

## Relationships

### Conforms To

- BidirectionalCollection
- Collection
- Comparable
- Copyable
- CustomDebugStringConvertible
- CustomReflectable
- CustomStringConvertible
- Decodable
- Encodable
- Equatable
- ExpressibleByArrayLiteral
- Hashable
- MutableCollection
- RandomAccessCollection
- ReferenceConvertible
- Sendable
- Sequence

## See Also

### Indexes

struct IndexSet

A collection of unique integer values that represent the indexes of elements in another collection.

