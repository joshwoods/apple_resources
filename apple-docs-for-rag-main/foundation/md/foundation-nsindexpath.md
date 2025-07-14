

- Foundation
-  NSIndexPath 

Class

# NSIndexPath

A list of indexes that together represent the path to a specific location in a tree of nested arrays.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
class NSIndexPath
```

## Overview

In Swift, this object bridges to IndexPath; use NSIndexPath when you need reference semantics or other Foundation-specific behavior.

Each index in an index path represents the index into an array of children from one node in the tree to another, deeper, node. For example, the index path `1.4.3.2` specifies the path shown in Figure 1.

Note

The UIKit framework adds programming interfaces to the `NSIndexPath` class of the Foundation framework to facilitate the identification of rows and sections in UITableView objects and the identification of items and sections in UICollectionView objects. The API consists of class factory methods and properties for accessing the various indexed values. You use the factory methods to create an index path for the corresponding table view or collection view.

Important

The Swift overlay to the Foundation framework provides the IndexPath structure, which bridges to the NSIndexPath class. For more information about value types, see Working with Cocoa Frameworks in Using Swift with Cocoa and Objective-C (Swift 4.1).

## Topics

### Creating and Initializing Index Paths

convenience init(index: Int)

Initializes an index path with a single node.

init(indexes: UnsafePointer&lt;Int>?, length: Int)

Initializes an index path with the given nodes and length.

### Using Special Node Names

UIKit and AppKit supply specialized names for the first two index path nodes for use when working with table views and collection views.

convenience init(forRow: Int, inSection: Int)

Initializes an index path with the indexes of a specific row and section in a table view.

convenience init(forItem: Int, inSection: Int)

Initializes an index path with the indexes of a specific item and section in a collection view.

var section: Int

An index number identifying a section in a table view or collection view.

var row: Int

An index number identifying a row in a section of a table view.

var item: Int

An index number identifying an item in a section of a collection view.

### Counting Nodes

var length: Int

The number of nodes in the index path.

### Adding and Removing Nodes

func adding(Int) -> IndexPath

Returns an index path containing the nodes in the receiving index path plus another given index.

func removingLastIndex() -> IndexPath

Returns an index path with the nodes in the receiving index path, excluding the last one.

### Comparing Index Paths

func compare(IndexPath) -> ComparisonResult

Indicates the depth-first traversal order of the receiving index path and another index path.

### Working with Indexes

func index(atPosition: Int) -> Int

Provides the value at a particular node in the index path.

func getIndexes(UnsafeMutablePointer&lt;Int>, range: NSRange)

Copies the indexes stored in the index path from the positions specified by the position range into the specified indexes.

func getIndexes(UnsafeMutablePointer&lt;Int>)

Copies the objects contained in the index path into indexes.

Deprecated

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- Copyable
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSCopying
- NSObjectProtocol
- NSSecureCoding

