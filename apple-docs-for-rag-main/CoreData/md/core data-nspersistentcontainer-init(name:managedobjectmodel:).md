

- Core Data
- NSPersistentContainer
-  init(name:managedObjectModel:) 

Initializer

# init(name:managedObjectModel:)

Create a container with the specified name and managed object model.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+watchOS 3.0+

``` source
init(
    name: String,
    managedObjectModel model: NSManagedObjectModel
)
```

## Parameters 

`name`  

The name used by the persistent container.

`model`  

The managed object model to be used by the persistent container.

## Return Value

A persistent container initialized with the given name and model.

## Discussion

By default, the provided name value of the container is used as the name of the persisent store associated with the container. Passing in the NSManagedObjectModel object overrides the lookup of the model by the provided name value.

## See Also

### Creating a Container

convenience init(name: String)

Creates a container with the specified name.

