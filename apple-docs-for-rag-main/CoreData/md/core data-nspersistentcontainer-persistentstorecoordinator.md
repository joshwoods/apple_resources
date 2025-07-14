

- Core Data
- NSPersistentContainer
-  persistentStoreCoordinator 

Instance Property

# persistentStoreCoordinator

The container’s persistent store coordinator.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+watchOS 3.0+

``` source
var persistentStoreCoordinator: NSPersistentStoreCoordinator { get }
```

## Mentioned in 

Setting up a Core Data stack

## Discussion

When the persistent container is initialized, it creates a persistent store coordinator as part of that initialization. That persistent store coordinator is referenced in this property.

## See Also

### Getting the Container’s Configuration

var managedObjectModel: NSManagedObjectModel

The container’s managed object model.

var name: String

The container’s name.

