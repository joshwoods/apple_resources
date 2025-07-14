

- Core Data
- NSManagedObject
-  entity() 

Type Method

# entity()

Returns the entity description that is associated with this subclass.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+watchOS 3.0+

``` source
class func entity() -> NSEntityDescription
```

## Discussion

This method is only legal to call on subclasses of `NSManagedObject` that represent a single entity in the model.

## See Also

### Getting a Managed Object’s Identity

var entity: NSEntityDescription

The entity description of the managed object.

var objectID: NSManagedObjectID

The object ID of the managed object.

