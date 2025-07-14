

- AppKit
- NSTreeController
-  move(\_:to:) 

Instance Method

# move(\_:to:)

Moves the specified tree nodes to the new index path.

macOS 10.5+

``` source
func move(
    _ nodes: [NSTreeNode],
    to startingIndexPath: IndexPath
)
```

## Parameters 

`nodes`  

An array of tree nodes.

`startingIndexPath`  

An index path specifying the starting position to move the tree nodes to in the tree controller’s content.

## See Also

### Adding, inserting and removing objects

func add(Any?)

Adds an object to the tree controller’s content after the current selection.

func addChild(Any?)

Adds a child object to the currently selected item.

var canAddChild: Bool

A Boolean value that indicates if a child object can be added to the tree controller’s content.

var canInsert: Bool

A Boolean value that indicates if an object can be inserted into the tree controller’s content.

var canInsertChild: Bool

A Boolean value that indicates if a child object can be inserted into the tree controller’s content.

func insert(Any?)

Creates a new object of the class specified by `objectClass` and inserts it into the tree controller’s content.

func insertChild(Any?)

Creates a new object of the class specified by `objectClass` and inserts it into the tree controller’s content as a child of the current selection.

func insert(Any?, atArrangedObjectIndexPath: IndexPath)

Inserts `object` into the tree controller’s arranged objects array at the location specified by `indexPath`, and adds it to the tree controller’s content.

func insert([Any], atArrangedObjectIndexPaths: [IndexPath])

Inserts `objects` into the tree controller’s arranged objects array at the locations specified in `indexPaths`, and adds them to the tree controller’s content.

func remove(Any?)

Removes the tree controller’s selected objects from the content.

func removeObject(atArrangedObjectIndexPath: IndexPath)

Removes the object at the specified `indexPath` in the tree controller’s arranged objects from the tree controller’s content.

func removeObjects(atArrangedObjectIndexPaths: [IndexPath])

Removes the objects at the specified `indexPaths` in the tree controller’s arranged objects from the tree controller’s content.

func move(NSTreeNode, to: IndexPath)

Moves the specified tree node to the new index path.

