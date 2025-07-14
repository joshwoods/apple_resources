

- Core Data
- NSManagedObjectModel
-  versionIdentifiers 

Instance Property

# versionIdentifiers

The set of developer-defined version identifiers for the object model.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.5+tvOSvisionOS 1.0+watchOS 2.0+

``` source
var versionIdentifiers: Set { get set }
```

## Discussion

Merged models return the combined collection of identifiers. The Core Data framework does not assign a default identifier to object models, nor does it depend on this value at runtime. For models you create in Xcode, set this value in the model inspector.

Use this value when debugging to help determine the models that Core Data merges to create the merged model.

## See Also

### Versioning and migrating entities

var versionChecksum: String

The Base64-encoded 128-bit model version hash.

var entityVersionHashesByName: [String : Data]

The dictionary of the model’s entity names and their corresponding version hashes.

func isConfiguration(withName: String?, compatibleWithStoreMetadata: [String : Any]) -> Bool

Returns a Boolean value that indicates whether a given configuration in the model is compatible with given metadata from a persistent store.

