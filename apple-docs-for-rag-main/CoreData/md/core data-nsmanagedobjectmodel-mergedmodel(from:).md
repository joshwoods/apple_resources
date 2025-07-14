

- Core Data
- NSManagedObjectModel
-  mergedModel(from:) 

Type Method

# mergedModel(from:)

Returns a model created by merging all the models found in given bundles.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.4+tvOSvisionOS 1.0+watchOS 2.0+

``` source
class func mergedModel(from bundles: [Bundle]?) -> NSManagedObjectModel?
```

## Parameters 

`bundles`  

An array of instances of `NSBundle` to search. If you specify `nil`, then the main bundle is searched.

## Return Value

A model created by merging all the models found in `bundles`.

## See Also

### Creating a managed object model

convenience init?(contentsOf: URL)

Initializes the managed object model using the model file at the specified URL.

init()

Initializes an empty managed object model.

class func mergedModel(from: [Bundle]?, forStoreMetadata: [String : Any]) -> NSManagedObjectModel?

Returns a merged model from a specified array for the version information in provided metadata.

init?(byMerging: [NSManagedObjectModel]?)

Creates a single model from an array of existing models.

init?(byMerging: [NSManagedObjectModel], forStoreMetadata: [String : Any])

Returns, for the version information in given metadata, a model merged from a given array of models.

