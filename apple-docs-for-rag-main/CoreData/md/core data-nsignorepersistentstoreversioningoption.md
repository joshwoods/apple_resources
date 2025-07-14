

- Core Data
-  NSIgnorePersistentStoreVersioningOption 

Global Variable

# NSIgnorePersistentStoreVersioningOption

Key to ignore the built-in versioning provided by Core Data.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.5+tvOSvisionOS 1.0+watchOS 2.0+

``` source
let NSIgnorePersistentStoreVersioningOption: String
```

## Discussion

The corresponding value is an `NSNumber` object. If the boolValue of the number is true, Core Data will not compare the version hashes between the managed object model in the coordinator and the metadata for the loaded store. (It will, however, continue to update the version hash information in the metadata.) This key and corresponding value of true is specified by default for all applications linked on or before OS X v10.4.

## See Also

### Constants

let NSMigratePersistentStoresAutomaticallyOption: String

Key to automatically attempt to migrate versioned stores.

let NSInferMappingModelAutomaticallyOption: String

Key to attempt to create the mapping model automatically.

