

- Core Data
- NSMappingModel
-  inferredMappingModel(forSourceModel:destinationModel:) 

Type Method

# inferredMappingModel(forSourceModel:destinationModel:)

Returns a newly created mapping model that will migrate data from the source to the destination model.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.6+tvOSvisionOS 1.0+watchOS 2.0+

``` source
class func inferredMappingModel(
    forSourceModel sourceModel: NSManagedObjectModel,
    destinationModel: NSManagedObjectModel
) throws -> NSMappingModel
```

## Parameters 

`sourceModel`  

The source managed object model.

`destinationModel`  

The destination managed object model.

## Return Value

A newly-created mapping model to migrate data from the source to the destination model. If the mapping model can not be created, returns `nil`.

## Mentioned in 

Migrating your data model automatically

## Discussion

A model will be created only if all changes are simple enough to be able to reasonably infer a mapping (for example, removing or renaming an attribute, adding an optional attribute or relationship, or adding renaming or deleting an entity). Element IDs are used to track renamed properties and entities.

## See Also

### Creating a Mapping

init?(from: [Bundle]?, forSourceModel: NSManagedObjectModel?, destinationModel: NSManagedObjectModel?)

Returns the mapping model that will translate data from the source to the destination model.

init?(contentsOf: URL?)

Returns a mapping model initialized from a given URL.

