

- Core Data
- NSPersistentContainer
-  managedObjectModel 

Instance Property

# managedObjectModel

The container’s managed object model.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+watchOS 3.0+

``` source
var managedObjectModel: NSManagedObjectModel { get }
```

## Mentioned in 

Setting up a Core Data stack

## Discussion

This property contains a reference to the NSManagedObjectModel object associated with this persistent container.

## See Also

### Getting the Container’s Configuration

var name: String

The container’s name.

var persistentStoreCoordinator: NSPersistentStoreCoordinator

The container’s persistent store coordinator.

