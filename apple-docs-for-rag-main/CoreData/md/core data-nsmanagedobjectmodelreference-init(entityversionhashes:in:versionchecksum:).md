

- Core Data
- NSManagedObjectModelReference
-  init(entityVersionHashes:in:versionChecksum:) 

Initializer

# init(entityVersionHashes:in:versionChecksum:)

Creates an object model reference with the entities corresponding to the specified entity version hashes.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
init(
    entityVersionHashes versionHash: [AnyHashable : Any],
    in bundle: Bundle?,
    versionChecksum: String
)
```

## Parameters 

`versionHash`  

The dictionary of entity names and their corresponding version hashes.

`bundle`  

The bundle to search.

`versionChecksum`  

The checksum of the object model’s version.

## Discussion

To determine an object model’s version checksum, use its versionChecksum property. Alternatively, you can find the checksum in the versioned model’s `VersionInfo.plist` file or in Xcode’s build log.

## See Also

### Creating a reference

init(model: NSManagedObjectModel, versionChecksum: String)

Creates an object model reference for the specified model.

init(fileURL: URL, versionChecksum: String)

Creates an object model reference for the model at the specified file URL.

init(name: String, in: Bundle?, versionChecksum: String)

Creates an object model reference for the named model in the specified bundle.

