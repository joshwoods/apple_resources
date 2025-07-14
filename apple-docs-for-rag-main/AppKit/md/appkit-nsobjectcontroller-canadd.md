

- AppKit
- NSObjectController
-  canAdd 

Instance Property

# canAdd

A Boolean value that indicates whether an object can be added to the receiver using add(_:).

macOS

``` source
var canAdd: Bool { get }
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

func remove(Any?)

Removes the receiver’s content object.

var canRemove: Bool

A Boolean value that indicates whether an object can be removed from the receiver.

