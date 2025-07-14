

- AppKit
- NSArrayController
-  remove(\_:) 

Instance Method

# remove(\_:)

Removes the receiver’s selected objects from the content collection.

macOS

``` source
@IBAction @MainActor
func remove(_ sender: Any?)
```

## Parameters 

`sender`  

Typically the object that invoked this method.

## Discussion

See removeObject(_:) for a discussion of the semantics of removing objects when using Core Data.

### Special Considerations

Beginning with OS X v10.4 the result of this method is deferred until the next iteration of the runloop so that the error presentation mechanism (see Error Responders and Error Recovery) can provide feedback as a sheet.

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

func removeObject(Any)

Removes `object` from the receiver’s content collection.

func remove(contentsOf: [Any])

Removes `objects` from the receiver’s content collection.

