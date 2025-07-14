

- Core Data
- NSManagedObject
-  entity 

Instance Property

# entity

The entity description of the managed object.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.4+tvOSvisionOS 1.0+watchOS 2.0+

``` source
var entity: NSEntityDescription { get }
```

## Discussion

If the receiver is a fault, accessing this property does not cause it to fire.

## See Also

### Getting a Managed Object’s Identity

var objectID: NSManagedObjectID

The object ID of the managed object.

class func entity() -> NSEntityDescription

Returns the entity description that is associated with this subclass.

