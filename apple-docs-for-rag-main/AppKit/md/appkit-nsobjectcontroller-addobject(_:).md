

- AppKit
- NSObjectController
-  addObject(\_:) 

Instance Method

# addObject(\_:)

Sets the receiver’s content object.

macOS

``` source
func addObject(_ object: Any)
```

## Parameters 

`object`  

The content object for the receiver.

## Discussion

If the receiver’s content is bound to another (primary) object or controller through a relationship key, the relationship of the primary object is changed. In a tree-like structure, the object is added after the current selection at the same depth. If there is no selection, the object is appended to the child nodes of the tree’s arranged objects.

## See Also

### Managing objects

func newObject() -> Any

Creates and returns a new object of the appropriate class.

func removeObject(Any)

Removes a given object from the receiver’s content.

func add(Any?)

Creates a new object and sets it as the receiver’s content object.

var canAdd: Bool

A Boolean value that indicates whether an object can be added to the receiver using add(_:).

func remove(Any?)

Removes the receiver’s content object.

var canRemove: Bool

A Boolean value that indicates whether an object can be removed from the receiver.

