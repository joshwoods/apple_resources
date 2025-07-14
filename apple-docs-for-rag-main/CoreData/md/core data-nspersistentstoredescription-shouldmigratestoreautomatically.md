

- Core Data
- NSPersistentStoreDescription
-  shouldMigrateStoreAutomatically 

Instance Property

# shouldMigrateStoreAutomatically

A flag indicating whether the associated persistent store should be migrated automatically.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+watchOS 3.0+

``` source
var shouldMigrateStoreAutomatically: Bool { get set }
```

## Discussion

If this is set to false and the store is out of sync, attempting to load the store produces an error. If this is set to true and the store is out of sync, attempting to load the store causes Core Data to attempt a migration. This flag is set to true by default.

## See Also

### Configuring a Persistent Store Description

var url: URL?

The URL that the store will use for its location.

var configuration: String?

The name of the configuration used by this store.

var timeout: TimeInterval

The connection timeout for the associated store.

var type: String

The type of store this description represents.

var isReadOnly: Bool

A flag that indicates whether this store will be read-only.

var shouldAddStoreAsynchronously: Bool

A flag that determines whether the store is added asynchronously.

var shouldInferMappingModelAutomatically: Bool

A flag indicating whether a mapping model should be created automatically.

func setOption(NSObject?, forKey: String)

Sets an option on the store.

func setValue(NSObject?, forPragmaNamed: String)

Allows you to set pragmas for the SQLite store.

