

- Core Data
- NSManagedObjectModel
-  init(byMerging:) 

Initializer

# init(byMerging:)

Creates a single model from an array of existing models.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.4+tvOSvisionOS 1.0+watchOS 2.0+

``` source
init?(byMerging models: [NSManagedObjectModel]?)
```

## Parameters 

`models`  

An array of instances of `NSManagedObjectModel`.

## Return Value

A single model made by combining the models in `models`.

## Discussion

You use this method to combine multiple models (typically from different frameworks) into one.

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

init?(byMerging: [NSManagedObjectModel], forStoreMetadata: [String : Any])

Returns, for the version information in given metadata, a model merged from a given array of models.

