

- AppKit
- NSObjectController
-  canRemove 

Instance Property

# canRemove

A Boolean value that indicates whether an object can be removed from the receiver.

macOS

``` source
var canRemove: Bool { get }
```

## Discussion

Bindings can use this method to control the enabling of user interface objects.

This property is observable using key-value observing.

## See Also

### Managing objects

func newObject() -> Any

Creates and returns a new object of the appropriate class.

func addObject(Any)

Sets the receiver’s content object.

func removeObject(Any)

Removes a given object from the receiver’s content.

func add(Any?)

Creates a new object and sets it as the receiver’s content object.

var canAdd: Bool

A Boolean value that indicates whether an object can be added to the receiver using add(_:).

func remove(Any?)

Removes the receiver’s content object.

