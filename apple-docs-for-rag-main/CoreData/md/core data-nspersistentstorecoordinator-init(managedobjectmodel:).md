

- Core Data
- NSPersistentStoreCoordinator
-  init(managedObjectModel:) 

Initializer

# init(managedObjectModel:)

Creates a persistent store coordinator with the specified managed object model.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.4+tvOSvisionOS 1.0+watchOS 2.0+

``` source
init(managedObjectModel model: NSManagedObjectModel)
```

## Parameters 

`model`  

A managed object model.

## Return Value

The receiver, initialized with `model`.

## See Also

### Creating a persistent store coordinator

Store options

The options keys that configure the behavior and characteristics of a persistent store.

Migration options

The options keys that configure the migration behavior of a persistent store.

Store versions

The metadata keys you use when comparing store versions.

