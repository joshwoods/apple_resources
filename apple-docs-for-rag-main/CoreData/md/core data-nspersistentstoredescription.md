

- Core Data
-  NSPersistentStoreDescription 

Class

# NSPersistentStoreDescription

A description object used to create and load a persistent store.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+watchOS 3.0+

``` source
class NSPersistentStoreDescription
```

## Mentioned in 

Setting Up Core Data with CloudKit

## Topics

### Creating a Persistent Store Description

init(url: URL)

Initializes the receiver with a URL for the store.

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

func setValue(NSObject?, forPragmaNamed: String)

Allows you to set pragmas for the SQLite store.

### Accessing the Configuration Options

var options: [String : NSObject]

A dictionary representation of the options set on the associated persistent store.

var sqlitePragmas: [String : NSObject]

The SQLite pragmas set for the associated persistent store. (read-only)

### Syncing to CloudKit

var cloudKitContainerOptions: NSPersistentCloudKitContainerOptions?

Options that customize how this store description aligns with a CloudKit database.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCopying
- NSObjectProtocol

## See Also

### Store Coordination

class NSPersistentStoreCoordinator

An object that enables an app’s contexts and the underlying persistent stores to work together.

class NSPersistentStore

The abstract base class for all Core Data persistent stores.

class NSPersistentStoreRequest

Criteria used to retrieve data from or save data to a persistent store.

class NSPersistentStoreResult

The abstract base class for results returned from a persistent store coordinator.

class NSPersistentStoreAsynchronousResult

A concrete class used to represent the results of an asynchronous request.

class NSSaveChangesRequest

An encapsulation of a collection of changes to be made by an object store in response to a save operation on a managed object context.

class NSAtomicStore

An abstract superclass that you subclass to create a Core Data atomic store.

class NSAtomicStoreCacheNode

A concrete class that you use to represent basic nodes in a Core Data atomic store.

class NSIncrementalStore

An abstract superclass defining the API through which Core Data communicates with a store.

class NSIncrementalStoreNode

A concrete class used to represent basic nodes in a Core Data incremental store.

