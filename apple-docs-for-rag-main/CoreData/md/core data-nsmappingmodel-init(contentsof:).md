

- Core Data
- NSMappingModel
-  init(contentsOf:) 

Initializer

# init(contentsOf:)

Returns a mapping model initialized from a given URL.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.5+tvOSvisionOS 1.0+watchOS 2.0+

``` source
init?(contentsOf url: URL?)
```

## Parameters 

`url`  

The location of an archived mapping model.

## Return Value

A mapping model initialized from `url`.

## See Also

### Creating a Mapping

init?(from: [Bundle]?, forSourceModel: NSManagedObjectModel?, destinationModel: NSManagedObjectModel?)

Returns the mapping model that will translate data from the source to the destination model.

class func inferredMappingModel(forSourceModel: NSManagedObjectModel, destinationModel: NSManagedObjectModel) throws -> NSMappingModel

Returns a newly created mapping model that will migrate data from the source to the destination model.

