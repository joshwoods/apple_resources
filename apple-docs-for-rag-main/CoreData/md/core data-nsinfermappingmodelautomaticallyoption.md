

- Core Data
-  NSInferMappingModelAutomaticallyOption 

Global Variable

# NSInferMappingModelAutomaticallyOption

Key to attempt to create the mapping model automatically.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.6+tvOSvisionOS 1.0+watchOS 2.0+

``` source
let NSInferMappingModelAutomaticallyOption: String
```

## Mentioned in 

Migrating your data model automatically

## Discussion

The corresponding value is an `NSNumber` object. If the boolValue of the number is true and the value of the `NSMigratePersistentStoresAutomaticallyOption` is true, the coordinator will attempt to infer a mapping model if none can be found.

## See Also

### Constants

let NSIgnorePersistentStoreVersioningOption: String

Key to ignore the built-in versioning provided by Core Data.

let NSMigratePersistentStoresAutomaticallyOption: String

Key to automatically attempt to migrate versioned stores.

