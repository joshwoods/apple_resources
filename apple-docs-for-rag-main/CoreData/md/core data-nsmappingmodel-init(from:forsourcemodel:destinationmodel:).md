

- Core Data
- NSMappingModel
-  init(from:forSourceModel:destinationModel:) 

Initializer

# init(from:forSourceModel:destinationModel:)

Returns the mapping model that will translate data from the source to the destination model.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.5+tvOSvisionOS 1.0+watchOS 2.0+

``` source
init?(
    from bundles: [Bundle]?,
    forSourceModel sourceModel: NSManagedObjectModel?,
    destinationModel: NSManagedObjectModel?
)
```

## Parameters 

`bundles`  

An array of bundles in which to search for mapping models.

`sourceModel`  

The managed object model for the source store.

`destinationModel`  

The managed object model for the destination store.

## Return Value

Returns the mapping model to translate data from `sourceModel` to `destinationModel`. If a suitable mapping model cannot be found, returns `nil`.

## Discussion

This method is a companion to the mergedModel(from:) and mergedModel(from:forStoreMetadata:) methods. In this case, the framework uses the version information from the models to locate the appropriate mapping model in the available bundles.

## See Also

### Related Documentation

Core Data Model Versioning and Data Migration Programming Guide

### Creating a Mapping

class func inferredMappingModel(forSourceModel: NSManagedObjectModel, destinationModel: NSManagedObjectModel) throws -> NSMappingModel

Returns a newly created mapping model that will migrate data from the source to the destination model.

init?(contentsOf: URL?)

Returns a mapping model initialized from a given URL.

