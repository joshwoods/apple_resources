

- AppKit
- NSTreeController
-  remove(\_:) 

Instance Method

# remove(\_:)

Removes the tree controller’s selected objects from the content.

macOS

``` source
@IBAction @MainActor
func remove(_ sender: Any?)
```

## Discussion

The `sender` is typically the object that invoked this method.

### Special Considerations

The result of this method is deferred until the next iteration of the run loop so that the error presentation mechanism can provide feedback as a sheet.

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

func removeObject(atArrangedObjectIndexPath: IndexPath)

Removes the object at the specified `indexPath` in the tree controller’s arranged objects from the tree controller’s content.

func removeObjects(atArrangedObjectIndexPaths: [IndexPath])

Removes the objects at the specified `indexPaths` in the tree controller’s arranged objects from the tree controller’s content.

func move(NSTreeNode, to: IndexPath)

Moves the specified tree node to the new index path.

func move([NSTreeNode], to: IndexPath)

Moves the specified tree nodes to the new index path.

