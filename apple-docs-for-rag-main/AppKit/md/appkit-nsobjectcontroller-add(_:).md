

- AppKit
- NSObjectController
-  add(\_:) 

Instance Method

# add(\_:)

Creates a new object and sets it as the receiver’s content object.

macOS

``` source
@IBAction @MainActor
func add(_ sender: Any?)
```

## Parameters 

`sender`  

Typically the object that invoked this method.

## Discussion

Creates a new object of the appropriate entity (specified by entityName) or class (specified by objectClass)—see newObject()—and sets it as the receiver’s content object using addObject(_:).

### Special Considerations

Beginning with OS X v10.4 the result of this method is deferred until the next iteration of the runloop so that the error presentation mechanism can provide feedback as a sheet.

## See Also

### Managing objects

func newObject() -> Any

Creates and returns a new object of the appropriate class.

func addObject(Any)

Sets the receiver’s content object.

func removeObject(Any)

Removes a given object from the receiver’s content.

var canAdd: Bool

A Boolean value that indicates whether an object can be added to the receiver using add(_:).

func remove(Any?)

Removes the receiver’s content object.

var canRemove: Bool

A Boolean value that indicates whether an object can be removed from the receiver.

