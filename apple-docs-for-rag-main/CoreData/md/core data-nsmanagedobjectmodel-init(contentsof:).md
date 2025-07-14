

- Core Data
- NSManagedObjectModel
-  init(contentsOf:) 

Initializer

# init(contentsOf:)

Initializes the managed object model using the model file at the specified URL.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.4+tvOSvisionOS 1.0+watchOS 2.0+

``` source
convenience init?(contentsOf url: URL)
```

## Parameters 

`url`  

An URL object specifying the location of a model file.

## Return Value

A managed object model initialized using the file at `url`.

## See Also

### Related Documentation

Core Data Programming Guide

Core Data Model Versioning and Data Migration Programming Guide

### Creating a managed object model

init()

Initializes an empty managed object model.

class func mergedModel(from: [Bundle]?) -> NSManagedObjectModel?

Returns a model created by merging all the models found in given bundles.

class func mergedModel(from: [Bundle]?, forStoreMetadata: [String : Any]) -> NSManagedObjectModel?

Returns a merged model from a specified array for the version information in provided metadata.

init?(byMerging: [NSManagedObjectModel]?)

Creates a single model from an array of existing models.

init?(byMerging: [NSManagedObjectModel], forStoreMetadata: [String : Any])

Returns, for the version information in given metadata, a model merged from a given array of models.

