

- AppKit
- NSObjectController
-  removeObject(\_:) 

Instance Method

# removeObject(\_:)

Removes a given object from the receiver’s content.

macOS

``` source
func removeObject(_ object: Any)
```

## Parameters 

`object`  

The object to remove from the receiver.

## Discussion

If `object` is the receiver’s content object, the receiver’s content is set to `nil`. If the receiver’s content is bound to another (primary) object or controller through a relationship key, the relationship of the primary object is cleared.

## See Also

### Managing objects

func newObject() -> Any

Creates and returns a new object of the appropriate class.

func addObject(Any)

Sets the receiver’s content object.

func add(Any?)

Creates a new object and sets it as the receiver’s content object.

var canAdd: Bool

A Boolean value that indicates whether an object can be added to the receiver using add(_:).

func remove(Any?)

Removes the receiver’s content object.

var canRemove: Bool

A Boolean value that indicates whether an object can be removed from the receiver.

