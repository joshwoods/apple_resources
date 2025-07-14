

- Core Data
- NSManagedObjectModel
-  mergedModel(from:forStoreMetadata:) 

Type Method

# mergedModel(from:forStoreMetadata:)

Returns a merged model from a specified array for the version information in provided metadata.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.5+tvOSvisionOS 1.0+watchOS 2.0+

``` source
class func mergedModel(
    from bundles: [Bundle]?,
    forStoreMetadata metadata: [String : Any]
) -> NSManagedObjectModel?
```

## Parameters 

`bundles`  

An array of bundles.

`metadata`  

A dictionary containing version information from the metadata for a persistent store.

## Return Value

The managed object model used to create the store for the metadata. If a model cannot be created to match the version information specified by `metadata`, returns `nil`.

## Discussion

This method is a companion to mergedModel(from:).

## See Also

### Creating a managed object model

convenience init?(contentsOf: URL)

Initializes the managed object model using the model file at the specified URL.

init()

Initializes an empty managed object model.

class func mergedModel(from: [Bundle]?) -> NSManagedObjectModel?

Returns a model created by merging all the models found in given bundles.

init?(byMerging: [NSManagedObjectModel]?)

Creates a single model from an array of existing models.

init?(byMerging: [NSManagedObjectModel], forStoreMetadata: [String : Any])

Returns, for the version information in given metadata, a model merged from a given array of models.

