

- Core Data
- NSPersistentStoreDescription
-  setValue(\_:forPragmaNamed:) 

Instance Method

# setValue(\_:forPragmaNamed:)

Allows you to set pragmas for the SQLite store.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+watchOS 3.0+

``` source
func setValue(
    _ value: NSObject?,
    forPragmaNamed name: String
)
```

## Parameters 

`value`  

The value of the pragma to be set.

`name`  

The name of the pragma to be set.

## Discussion

Pragma options are for SQLite stores only. All pragma values must be specified as NSStringobjects. The `fullfsync` and `synchronous` pragmas control the tradeoff between write performance (write to disk speed and cache utilization) and durability (data loss/corruption sensitivity to power interruption). For more information on pragma settings, see http://sqlite.org/pragma.html.

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

func setOption(NSObject?, forKey: String)

Sets an option on the store.

