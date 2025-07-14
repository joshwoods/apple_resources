

- AppKit
- NSObjectController
-  newObject() 

Instance Method

# newObject()

Creates and returns a new object of the appropriate class.

macOS

``` source
func newObject() -> Any
```

## Return Value

A new object of the appropriate class. The returned object is implicitly retained, the sender is responsible for releasing it (with either release or autorelease).

## Discussion

If an entity name is set (see entityName), the object created is an instance of the class specified for that entity (and the object is inserted into the receiver’s managed object context). Otherwise the object created is an instance of the class returned by objectClass.

This method is called when adding and inserting objects if automaticallyPreparesContent is true.

The default implementation assumes the class returned by objectClass has a standard `init` method without arguments. If the object class being controlled is `NSManagedObject` (or a subclass thereof) its designated initializer (init(entity:insertInto:)) is called instead, using the entity and managed object context specified for the receiver.

## See Also

### Related Documentation

var objectClass: AnyClass!

The object class to use when creating new objects.

var entityName: String?

The entity name used by the receiver to create new objects.

### Managing objects

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

var canRemove: Bool

A Boolean value that indicates whether an object can be removed from the receiver.

