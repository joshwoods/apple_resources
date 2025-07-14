

- Core Data
- NSMigrationManager
-  destinationInstances(forEntityMappingName:sourceInstances:) 

Instance Method

# destinationInstances(forEntityMappingName:sourceInstances:)

Returns the managed object instances created in the destination store for the named entity mapping for the given array of source instances.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.5+tvOSvisionOS 1.0+watchOS 2.0+

``` source
func destinationInstances(
    forEntityMappingName mappingName: String,
    sourceInstances: [NSManagedObject]?
) -> [NSManagedObject]
```

## Parameters 

`mappingName`  

The name of an entity mapping in use.

`sourceInstances`  

A array of managed objects in the source store.

## Return Value

An array containing the managed object instances created in the destination store for the entity mapping named `mappingName` for `sourceInstances`. If `sourceInstances` is `nil`, all of the destination instances created by the specified property mapping are returned.

## Discussion

This method throws an `NSInvalidArgumentException` exception if `mappingName` is not a valid mapping name.

## See Also

### Managing Sources and Destinations

func associate(sourceInstance: NSManagedObject, withDestinationInstance: NSManagedObject, for: NSEntityMapping)

Associates a given source managed object instance with an array of destination instances for a given property mapping.

func sourceInstances(forEntityMappingName: String, destinationInstances: [NSManagedObject]?) -> [NSManagedObject]

Returns the managed object instances in the source store used to create the given destination instances for the passed in property mapping.

