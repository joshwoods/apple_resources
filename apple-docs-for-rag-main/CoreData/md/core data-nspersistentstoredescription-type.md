

- Core Data
- NSPersistentStoreDescription
-  type 

Instance Property

# type

The type of store this description represents.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+watchOS 3.0+

``` source
var type: String { get set }
```

## Discussion

A string constant (such as `NSSQLiteStoreType`) that specifies the type of the new store—see NSPersistentStoreCoordinator.

## See Also

### Configuring a Persistent Store Description

var url: URL?

The URL that the store will use for its location.

var configuration: String?

The name of the configuration used by this store.

var timeout: TimeInterval

The connection timeout for the associated store.

var isReadOnly: Bool

A flag that indicates whether this store will be read-only.

var shouldAddStoreAsynchronously: Bool

A flag that determines whether the store is added asynchronously.

var shouldInferMappingModelAutomatically: Bool

A flag indicating whether a mapping model should be created automatically.

var shouldMigrateStoreAutomatically: Bool

A flag indicating whether the associated persistent store should be migrated automatically.

func setOption(NSObject?, forKey: String)

Sets an option on the store.

func setValue(NSObject?, forPragmaNamed: String)

Allows you to set pragmas for the SQLite store.

