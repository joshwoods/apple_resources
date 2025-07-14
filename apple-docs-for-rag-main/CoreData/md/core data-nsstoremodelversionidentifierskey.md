

- Core Data
-  NSStoreModelVersionIdentifiersKey 

Global Variable

# NSStoreModelVersionIdentifiersKey

Key to represent the version identifiers for the model used to create the store.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.5+tvOSvisionOS 1.0+watchOS 2.0+

``` source
let NSStoreModelVersionIdentifiersKey: String
```

## Discussion

If you add your own annotations to a model’s version identifier (see versionIdentifiers), they are stored in the persistent store’s metadata. You can use this key to retrieve the identifiers from the metadata dictionaries available from `NSPersistentStore` (metadata) and `NSPersistentStoreCoordinator` (metadata(for:) and related methods). The corresponding value is a Foundation collection (an `NSArray` or `NSSet` object).

## See Also

### Constants

let NSStoreModelVersionHashesKey: String

Key to represent the version hash information for the model used to create the store.

let NSPersistentStoreOSCompatibility: String

Key to represent the earliest version of the operation system that the persistent store supports.

