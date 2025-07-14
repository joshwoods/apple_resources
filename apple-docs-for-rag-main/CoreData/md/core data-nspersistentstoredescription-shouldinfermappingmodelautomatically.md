

- Core Data
- NSPersistentStoreDescription
-  shouldInferMappingModelAutomatically 

Instance Property

# shouldInferMappingModelAutomatically

A flag indicating whether a mapping model should be created automatically.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+watchOS 3.0+

``` source
var shouldInferMappingModelAutomatically: Bool { get set }
```

## Discussion

If this flag is set to true and the value of the shouldMigrateStoreAutomatically is true, the coordinator attempts to infer a mapping model if none can be found. The default for this flag is true.

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

var shouldMigrateStoreAutomatically: Bool

A flag indicating whether the associated persistent store should be migrated automatically.

func setOption(NSObject?, forKey: String)

Sets an option on the store.

func setValue(NSObject?, forPragmaNamed: String)

Allows you to set pragmas for the SQLite store.

