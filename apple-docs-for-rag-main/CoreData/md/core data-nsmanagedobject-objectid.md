

- Core Data
- NSManagedObject
-  objectID 

Instance Property

# objectID

The object ID of the managed object.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.4+tvOSvisionOS 1.0+watchOS 2.0+

``` source
var objectID: NSManagedObjectID { get }
```

## Mentioned in 

Consuming relevant store changes

Creating a Core Data Model for CloudKit

## Discussion

If the receiver is a fault, accessing this property does not cause it to fire.

Important

If the receiver has not yet been saved, the object ID is a temporary value that will change when the object is saved.

## See Also

### Related Documentation

func uriRepresentation() -> URL

Returns a URI that provides an archiveable reference to the object for the object ID.

### Getting a Managed Object’s Identity

var entity: NSEntityDescription

The entity description of the managed object.

class func entity() -> NSEntityDescription

Returns the entity description that is associated with this subclass.

