

- AppKit
- NSArrayController
-  add(contentsOf:) 

Instance Method

# add(contentsOf:)

Adds `objects` to the receiver’s content collection.

macOS

``` source
func add(contentsOf objects: [Any])
```

## Discussion

If selectsInsertedObjects is true (the default), the added objects are selected in the array controller.

It is important to note that inserting many objects with selectsInsertedObjects on can cause a significant performance penalty. In this case it is more efficient to use the content method to set the array, or to set selectsInsertedObjects to false before adding the objects with add(contentsOf:).

## See Also

### Adding and Removing Objects

func addObject(Any)

Adds `object` to the receiver’s content collection and the arranged objects array.

func insert(Any, atArrangedObjectIndex: Int)

Inserts `object` into the receiver’s arranged objects array at the location specified by `index`, and adds it to the receiver’s content collection.

func insert(contentsOf: [Any], atArrangedObjectIndexes: IndexSet)

Inserts `object`s into the receiver’s arranged objects array at the locations specified in `indexes`, and adds it to the receiver’s content collection.

func remove(atArrangedObjectIndex: Int)

Removes the object at the specified `index` in the receiver’s arranged objects from the receiver’s content array.

func remove(atArrangedObjectIndexes: IndexSet)

Removes the objects at the specified `indexes` in the receiver’s arranged objects from the content array.

func remove(Any?)

Removes the receiver’s selected objects from the content collection.

func removeObject(Any)

Removes `object` from the receiver’s content collection.

func remove(contentsOf: [Any])

Removes `objects` from the receiver’s content collection.

