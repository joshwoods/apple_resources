

- Core Data
- NSPersistentContainer
-  init(name:) 

Initializer

# init(name:)

Creates a container with the specified name.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+watchOS 3.0+

``` source
convenience init(name: String)
```

## Parameters 

`name`  

The name of the NSPersistentContainer object.

## Return Value

A persistent container initialized with the given name.

## Discussion

By default, the provided name value is used to name the persistent store and is used to look up the name of the NSManagedObjectModel object to be used with the NSPersistentContainer object.

## See Also

### Creating a Container

init(name: String, managedObjectModel: NSManagedObjectModel)

Create a container with the specified name and managed object model.

