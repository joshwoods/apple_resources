

- Core Data
- NSPersistentStoreDescription
-  setOption(\_:forKey:) 

Instance Method

# setOption(\_:forKey:)

Sets an option on the store.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+watchOS 3.0+

``` source
func setOption(
    _ option: NSObject?,
    forKey key: String
)
```

## Parameters 

`option`  

The value to be set for an option on the store.

`key`  

The key of the value to be set for an option on the store.

## Discussion

If a value was previously set for the given option, that value is replaced with the given value. Note that the keys are case-sensitive. For a list of the available options, see NSPersistentStoreCoordinator.

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

var shouldMigrateStoreAutomatically: Bool

A flag indicating whether the associated persistent store should be migrated automatically.

func setValue(NSObject?, forPragmaNamed: String)

Allows you to set pragmas for the SQLite store.

