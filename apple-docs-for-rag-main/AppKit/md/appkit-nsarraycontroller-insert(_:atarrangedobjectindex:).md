

- AppKit
- NSArrayController
-  insert(\_:atArrangedObjectIndex:) 

Instance Method

# insert(\_:atArrangedObjectIndex:)

Inserts `object` into the receiver’s arranged objects array at the location specified by `index`, and adds it to the receiver’s content collection.

macOS

``` source
func insert(
    _ object: Any,
    atArrangedObjectIndex index: Int
)
```

## Discussion

Subclasses can override this method to provide customized arranged objects support. An error is returned if the given index is outside of the arrangedObjects range, or if the given object would not appear in the arrangedObjects. Set the clearsFilterPredicateOnInsertion to true to allow insertion.

## See Also

### Adding and Removing Objects

func addObject(Any)

Adds `object` to the receiver’s content collection and the arranged objects array.

func add(contentsOf: [Any])

Adds `objects` to the receiver’s content collection.

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

