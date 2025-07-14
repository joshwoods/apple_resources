

- Core Data
- NSManagedObjectModel
-  entityVersionHashesByName 

Instance Property

# entityVersionHashesByName

The dictionary of the model’s entity names and their corresponding version hashes.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.5+tvOSvisionOS 1.0+watchOS 2.0+

``` source
var entityVersionHashesByName: [String : Data] { get }
```

## Discussion

Core Data use the dictionary of version hash information is to determine schema compatibility.

## See Also

### Versioning and migrating entities

var versionChecksum: String

The Base64-encoded 128-bit model version hash.

var versionIdentifiers: Set&lt;AnyHashable>

The set of developer-defined version identifiers for the object model.

func isConfiguration(withName: String?, compatibleWithStoreMetadata: [String : Any]) -> Bool

Returns a Boolean value that indicates whether a given configuration in the model is compatible with given metadata from a persistent store.

