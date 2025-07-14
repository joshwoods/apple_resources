

- Core Data
- Core Data stack
- NSPersistentStoreCoordinator
-  Spotlight record keys 

API Collection

# Spotlight record keys

The keys for the values that exist in Spotlight’s external record files.

## Topics

### Constants

let NSEntityNameInPathKey: String

Dictionary key for the entity name extracted from an external record file.

Deprecated

let NSStoreUUIDInPathKey: String

Dictionary key for the store UUID extracted from an external record file.

Deprecated

let NSStorePathKey: String

Dictionary key for the store path (an instance of `NSURL`) extracted from an external record file.

Deprecated

let NSModelPathKey: String

Dictionary key for the managed object model path (an instance of `NSURL`) extracted from an external record file.

Deprecated

let NSObjectURIKey: String

Dictionary key for the object URI extracted from an external record file.

Deprecated

## See Also

### Integrating with Spotlight

let NSCoreDataCoreSpotlightExporter: String

The key you use to specify your Core Spotlight delegate.

class NSCoreDataCoreSpotlightDelegate

A set of methods that enable integration with Core Spotlight.

Showcase App Data in Spotlight

Index app data so users can find it by using Spotlight search.

