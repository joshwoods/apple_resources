

- Core Foundation
-  CFTree 

Class

# CFTree

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
class CFTree
```

## Overview

You use CFTree to create tree structures that represent hierarchical organizations of information. In such structures, each tree node has exactly one parent tree (except for the root tree, which has no parent) and can have multiple children. Each CFTree object in the structure has a context associated with it; this context includes some program-defined data as well as callbacks that operate on that data. The program-defined data is often used as the basis for determining where CFTree objects fit within the structure. All CFTree objects are mutable.

You create a CFTree object using the CFTreeCreate(_:_:) function. This function takes an allocator and pointer to a CFTreeGetContext(_:_:) structure as parameters. The CFTreeContext structure contains the program-defined data and callbacks needed to describe, retain, and release that data. If you do not implement these callbacks, your program-defined data will not be retained or released when trees are added and removed from a parent.

Each CFTree object has a parent and list of children, all of which may be `NULL`. CFTree provides functions for adding and removing tree objects from the tree structure. Use the CFTreeAppendChild(_:_:), CFTreeInsertSibling(_:_:), or CFTreePrependChild(_:_:) functions to add trees to a tree structure, and the CFTreeRemove(_:) or CFTreeRemoveAllChildren(_:) functions to remove trees.

For the purposes of memory management, CFTree can be thought of as a collection. Typically the only object that retains a child tree is its parent. Usually, therefore, when you remove a child tree from a tree, the child tree is destroyed. If you want to use a child tree after you remove it from its parent, you should retain the child tree first, prior to removing it.

Releasing a tree releases its child trees, and all of their child trees (recursively). Note also that the final release of a tree (when its retain count decreases to zero) causes all of its child trees, and all of their child trees (recursively), to be destroyed, regardless of their retain counts. Releasing a child that is still in a tree is therefore a programming error, and may cause your application to crash.

You can use any of the get functions (functions containing the word “Get”) to obtain the parent, children, or attributes of a tree. For example, use CFTreeGetChildAtIndex(_:_:) to obtain a child of a tree at a specified location. In common with other Core Foundation “Get” functions, these functions do not retain the tree that is returned. If you are making other modifications to the tree, you should either retain or make a deep copy of the child tree returned.

You can apply a function to all children of a tree using the CFTreeApplyFunctionToChildren(_:_:_:) function, and sort children of a tree using the CFTreeSortChildren(_:_:_:) function.

## Topics

### Creating Trees

func CFTreeCreate(CFAllocator!, UnsafePointer&lt;CFTreeContext>!) -> CFTree!

Creates a new CFTree object.

### Modifying a Tree

func CFTreeAppendChild(CFTree!, CFTree!)

Adds a new child to a tree as the last in its list of children.

func CFTreeInsertSibling(CFTree!, CFTree!)

Inserts a new sibling after a given tree.

func CFTreeRemoveAllChildren(CFTree!)

Removes all the children of a tree.

func CFTreePrependChild(CFTree!, CFTree!)

Adds a new child to the specified tree as the first in its list of children.

func CFTreeRemove(CFTree!)

Removes a tree from its parent.

func CFTreeSetContext(CFTree!, UnsafePointer&lt;CFTreeContext>!)

Replaces the context of a tree by releasing the old information pointer and retaining the new one.

### Sorting a Tree

func CFTreeSortChildren(CFTree!, CFComparatorFunction!, UnsafeMutableRawPointer!)

Sorts the immediate children of a tree using a specified comparator function.

### Examining a Tree

func CFTreeFindRoot(CFTree!) -> CFTree!

Returns the root tree of a given tree.

func CFTreeGetChildAtIndex(CFTree!, CFIndex) -> CFTree!

Returns the child of a tree at the specified index.

func CFTreeGetChildCount(CFTree!) -> CFIndex

Returns the number of children in a tree.

func CFTreeGetChildren(CFTree!, UnsafeMutablePointer&lt;Unmanaged&lt;CFTree>?>!)

Fills a buffer with children from the tree.

func CFTreeGetContext(CFTree!, UnsafeMutablePointer&lt;CFTreeContext>!)

Returns the context of the specified tree.

func CFTreeGetFirstChild(CFTree!) -> CFTree!

Returns the first child of a tree.

func CFTreeGetNextSibling(CFTree!) -> CFTree!

Returns the next sibling, adjacent to a given tree, in the parent’s children list.

func CFTreeGetParent(CFTree!) -> CFTree!

Returns the parent of a given tree.

### Performing an Operation on Tree Elements

func CFTreeApplyFunctionToChildren(CFTree!, ((UnsafeRawPointer?, UnsafeMutableRawPointer?) -> Void)!, UnsafeMutableRawPointer!)

Calls a function once for each immediate child of a tree.

### Getting the Tree Type ID

func CFTreeGetTypeID() -> CFTypeID

Returns the type identifier of the CFTree opaque type.

### Callbacks

typealias CFTreeApplierFunction

Type of the callback function used by the CFTree apply function.

typealias CFTreeCopyDescriptionCallBack

Callback function used to provide a description of the program-defined information pointer.

typealias CFTreeReleaseCallBack

Callback function used to release a previously retained program-defined information pointer.

typealias CFTreeRetainCallBack

Callback function used to retain a program-defined information pointer.

### Data Types

struct CFTreeContext

Structure containing program-defined data and callbacks for a CFTree object.

## Relationships

### Conforms To

- Equatable
- Hashable

## See Also

### Related Documentation

Collections Programming Topics for Core Foundation

### Opaque Types

class CFAllocator

class CFArray

class CFAttributedString

class CFBag

class CFBinaryHeap

class CFBitVector

class CFBoolean

class CFBundle

class CFCalendar

class CFCharacterSet

class CFData

class CFDate

class CFDateFormatter

class CFDictionary

class CFError

