

- Core Data
-  NSMigratePersistentStoresAutomaticallyOption 

Global Variable

# NSMigratePersistentStoresAutomaticallyOption

Key to automatically attempt to migrate versioned stores.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.5+tvOSvisionOS 1.0+watchOS 2.0+

``` source
let NSMigratePersistentStoresAutomaticallyOption: String
```

## Mentioned in 

Migrating your data model automatically

## Discussion

The corresponding value is an `NSNumber` object. If the boolValue of the number is true and if the version hash information for the added store is determined to be incompatible with the model for the coordinator, Core Data will attempt to locate the source and mapping models in the application bundles, and perform a migration.

## See Also

### Constants

let NSIgnorePersistentStoreVersioningOption: String

Key to ignore the built-in versioning provided by Core Data.

let NSInferMappingModelAutomaticallyOption: String

Key to attempt to create the mapping model automatically.

