

- AppKit
- NSArrayController
-  removeObject(\_:) 

Instance Method

# removeObject(\_:)

Removes `object` from the receiver’s content collection.

macOS

``` source
func removeObject(_ object: Any)
```

## Discussion

If you are using Core Data, the exact semantics of this method differ depending on the settings for the array controller. If the receiver’s content is fetched automatically, removed objects are marked for deletion by the managed object context (and hence removal from the object graph). If, however, the receiver’s `contentSet` is bound to a relationship, `removeObject:` by default only removes the object from the relationship (not from the object graph). You can, though, set the “Deletes Object on Remove” option for the `contentSet` binding, in which case objects are marked for deletion as well as being removed from the relationship.

## See Also

### Adding and Removing Objects

func addObject(Any)

Adds `object` to the receiver’s content collection and the arranged objects array.

func add(contentsOf: [Any])

Adds `objects` to the receiver’s content collection.

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

func remove(contentsOf: [Any])

Removes `objects` from the receiver’s content collection.

