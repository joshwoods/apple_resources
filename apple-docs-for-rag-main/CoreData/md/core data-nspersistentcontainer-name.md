

- Core Data
- NSPersistentContainer
-  name 

Instance Property

# name

The container’s name.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+watchOS 3.0+

``` source
var name: String { get }
```

## Discussion

This property is passed in as part of the initialization of the persistent container. This name is used to locate the NSManagedObjectModel (if the NSManagedObjectModel object is not passed in as part of the initialization) and is used to name the persistent store.

## See Also

### Getting the Container’s Configuration

var managedObjectModel: NSManagedObjectModel

The container’s managed object model.

var persistentStoreCoordinator: NSPersistentStoreCoordinator

The container’s persistent store coordinator.

