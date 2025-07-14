

- Core Data
- NSManagedObjectModel
-  isConfiguration(withName:compatibleWithStoreMetadata:) 

Instance Method

# isConfiguration(withName:compatibleWithStoreMetadata:)

Returns a Boolean value that indicates whether a given configuration in the model is compatible with given metadata from a persistent store.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.5+tvOSvisionOS 1.0+watchOS 2.0+

``` source
func isConfiguration(
    withName configuration: String?,
    compatibleWithStoreMetadata metadata: [String : Any]
) -> Bool
```

## Parameters 

`configuration`  

The name of a configuration in the receiver. Pass `nil` to specify no configuration.

`metadata`  

Metadata for a persistent store.

## Return Value

true if the configuration in the receiver specified by `configuration` is compatible with the store metadata given by `metadata`, otherwise false.

## Discussion

This method compares the version information in the store metadata with the entity versions of a given configuration. For information on specific differences, use entityVersionHashesByName and perform an entity-by-entity comparison.

## See Also

### Versioning and migrating entities

var versionChecksum: String

The Base64-encoded 128-bit model version hash.

var versionIdentifiers: Set&lt;AnyHashable>

The set of developer-defined version identifiers for the object model.

var entityVersionHashesByName: [String : Data]

The dictionary of the model’s entity names and their corresponding version hashes.

