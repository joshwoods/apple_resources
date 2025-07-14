

- AppKit
-  NSTreeNode 

Class

# NSTreeNode

A node in a tree of nodes.

macOS 10.5+

``` source
class NSTreeNode
```

## Overview

NSTreeNode simplifies the creation and management of trees of objects. Each tree node represents a model object. A tree node with `nil` as its parent node is considered the root of the tree.

## Topics

### Creating tree nodes

init(representedObject: Any?)

Initializes a newly allocated tree node that represents the specified object.

### Getting information about a node

var representedObject: Any?

The object the tree node represents.

var indexPath: IndexPath

The position of the receiver relative to its root parent.

var isLeaf: Bool

A Boolean that indicates whether the receiver is a leaf node.

var children: [NSTreeNode]?

An array containing receiver’s child nodes.

var mutableChildren: NSMutableArray

A mutable array that provides read-write access to the receiver’s child nodes.

func descendant(at: IndexPath) -> NSTreeNode?

Returns the receiver’s descendant at the specified index path.

var parent: NSTreeNode?

The receiver’s parent node.

### Sorting the subtree

func sort(with: [NSSortDescriptor], recursively: Bool)

Sorts the receiver’s subtree using the values of the represented objects with the specified sort descriptors.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Tree-Based Data

Navigating Hierarchical Data Using Outline and Split Views

Build a structured user interface that simplifies navigation in your app.

class NSTreeController

A bindings-compatible controller that manages a tree of objects.

