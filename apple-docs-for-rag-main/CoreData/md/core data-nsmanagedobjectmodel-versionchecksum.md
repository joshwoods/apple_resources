

- Core Data
- NSManagedObjectModel
-  versionChecksum 

Instance Property

# versionChecksum

The Base64-encoded 128-bit model version hash.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
var versionChecksum: String { get }
```

## Discussion

This value is also available in the versioned model’s `VersionInfo.plist` file and in Xcode’s build log.

## See Also

### Versioning and migrating entities

var versionIdentifiers: Set&lt;AnyHashable>

The set of developer-defined version identifiers for the object model.

var entityVersionHashesByName: [String : Data]

The dictionary of the model’s entity names and their corresponding version hashes.

func isConfiguration(withName: String?, compatibleWithStoreMetadata: [String : Any]) -> Bool

Returns a Boolean value that indicates whether a given configuration in the model is compatible with given metadata from a persistent store.

