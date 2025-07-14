

- Core Data
- NSManagedObjectModel
-  init(byMerging:forStoreMetadata:) 

Initializer

# init(byMerging:forStoreMetadata:)

Returns, for the version information in given metadata, a model merged from a given array of models.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.5+tvOSvisionOS 1.0+watchOS 2.0+

``` source
init?(
    byMerging models: [NSManagedObjectModel],
    forStoreMetadata metadata: [String : Any]
)
```

## Parameters 

`models`  

An array of instances of `NSManagedObjectModel`.

`metadata`  

A dictionary containing version information from the metadata for a persistent store.

## Return Value

A merged model from `models` for the version information in `metadata`. If a model cannot be created to match the version information in `metadata`, returns `nil`.

## Discussion

This is the companion method to mergedModel(from:forStoreMetadata:).

## See Also

### Creating a managed object model

convenience init?(contentsOf: URL)

Initializes the managed object model using the model file at the specified URL.

init()

Initializes an empty managed object model.

class func mergedModel(from: [Bundle]?) -> NSManagedObjectModel?

Returns a model created by merging all the models found in given bundles.

class func mergedModel(from: [Bundle]?, forStoreMetadata: [String : Any]) -> NSManagedObjectModel?

Returns a merged model from a specified array for the version information in provided metadata.

init?(byMerging: [NSManagedObjectModel]?)

Creates a single model from an array of existing models.

