

- Core Data
-  NSPersistentStoreCoordinator 

Class

# NSPersistentStoreCoordinator

An object that enables an app’s contexts and the underlying persistent stores to work together.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.4+tvOSvisionOS 1.0+watchOS 2.0+

``` source
class NSPersistentStoreCoordinator
```

## Mentioned in 

Setting up a Core Data stack manually

Setting up a Core Data stack

## Overview

A managed object context uses a coordinator to facilitate the persistence of its entities in the coordinator’s registered stores. A context can’t function without a coordinator because it relies on the coordinator’s access to the managed object model. The coordinator presents its registered stores as an aggregate, allowing a context to operate on the union of those stores instead of on each individually. A coordinator performs its work on a private queue and executes that work serially. You can use multiple coordinators if the work requires separate queues.

Use a coordinator to add or remove persistent stores, change the type or location on-disk of those stores, query the metadata of a specific store, defer a store’s migrations, determine whether two objects originate from the same store, and so on.

## Topics

### Creating a persistent store coordinator

init(managedObjectModel: NSManagedObjectModel)

Creates a persistent store coordinator with the specified managed object model.

Store options

The options keys that configure the behavior and characteristics of a persistent store.

Migration options

The options keys that configure the migration behavior of a persistent store.

Store versions

The metadata keys you use when comparing store versions.

### Managing configuration

var name: String?

The coordinator’s name.

var managedObjectModel: NSManagedObjectModel

The coordinator’s managed object model.

var persistentStores: [NSPersistentStore]

The coordinator’s persistent stores.

### Registering store types

class func registerStoreClass(AnyClass?, type: NSPersistentStore.StoreType)

Registers a persistent store subclass using the specified store type.

class func registerStoreClass(AnyClass?, forStoreType: String)

Registers a persistent store subclass using the specified store type identifier.

Deprecated

class var registeredStoreTypes: [String : NSValue]

The coordinator’s registered store types.

### Adding or removing a store

func addPersistentStore(type: NSPersistentStore.StoreType, configuration: String?, at: URL, options: [AnyHashable : Any]?) throws -> NSPersistentStore

Adds a specific type of persistent store at the provided location.

func addPersistentStore(ofType: String, configurationName: String?, at: URL?, options: [AnyHashable : Any]?) throws -> NSPersistentStore

Adds a specific type of persistent store at the provided location.

Deprecated

func addPersistentStore(with: NSPersistentStoreDescription, completionHandler: (NSPersistentStoreDescription, (any Error)?) -> Void)

Adds a persistent store using the provided description.

func remove(NSPersistentStore) throws

Removes the specified persistent store from the coordinator.

### Modifying a store

func destroyPersistentStore(at: URL, type: NSPersistentStore.StoreType, options: [AnyHashable : Any]?) throws

Deletes a specific type of persistent store at the provided location.

func migratePersistentStore(NSPersistentStore, to: URL, options: [AnyHashable : Any]?, type: NSPersistentStore.StoreType) throws -> NSPersistentStore

Changes the location and, if necessary, the store type of the specified persistent store.

func replacePersistentStore(at: URL, destinationOptions: [AnyHashable : Any]?, withPersistentStoreFrom: URL, sourceOptions: [AnyHashable : Any]?, type: NSPersistentStore.StoreType) throws

Replaces one persistent store with another.

func destroyPersistentStore(at: URL, ofType: String, options: [AnyHashable : Any]?) throws

Deletes a specific type of persistent store at the provided location.

Deprecated

func migratePersistentStore(NSPersistentStore, to: URL, options: [AnyHashable : Any]?, withType: String) throws -> NSPersistentStore

Changes the location and, if necessary, the store type of the specified persistent store.

Deprecated

func replacePersistentStore(at: URL, destinationOptions: [AnyHashable : Any]?, withPersistentStoreFrom: URL, sourceOptions: [AnyHashable : Any]?, ofType: String) throws

Replaces one persistent store with another.

Deprecated

### Managing a store’s location

func setURL(URL, for: NSPersistentStore) -> Bool

Changes the location of the specified persistent store.

func persistentStore(for: URL) -> NSPersistentStore?

Returns the persistent store for the specified file URL.

func url(for: NSPersistentStore) -> URL

Returns the location of the provided persistent store.

### Managing a store’s metadata

class func setMetadata([String : Any]?, type: NSPersistentStore.StoreType, at: URL, options: [AnyHashable : Any]?) throws

Updates the metadata of a specific type of persistent store at the provided location.

class func metadataForPersistentStore(type: NSPersistentStore.StoreType, at: URL, options: [AnyHashable : Any]?) throws -> [String : Any]

Returns the metadata of a specific type of persistent store at the provided location.

class func setMetadata([String : Any]?, forPersistentStoreOfType: String, at: URL, options: [AnyHashable : Any]?) throws

Updates the metadata of a specific type of persistent store at the provided location.

Deprecated

class func metadataForPersistentStore(ofType: String, at: URL, options: [AnyHashable : Any]?) throws -> [String : Any]

Returns the metadata of a specific type of persistent store at the provided location.

Deprecated

func metadata(for: NSPersistentStore) -> [String : Any]

Returns the metadata of the specified persistent store.

func setMetadata([String : Any]?, for: NSPersistentStore)

Updates the metadata for the specified persistent store.

let NSStoreTypeKey: String

A key that identifies the store type.

let NSStoreUUIDKey: String

A key that provides the store’s UUID.

### Deferring a store’s migrations

let NSPersistentStoreDeferredLightweightMigrationOptionKey: String

The key for enabling deferred lightweight migrations.

func finishDeferredLightweightMigrationTask() throws

Executes a single pending task of a deferred lightweight migration.

func finishDeferredLightweightMigration() throws

Executes all remaining tasks of a deferred lightweight migration.

### Performing tasks

func perform&lt;T>(() throws -> T) async rethrows -> T

Executes the provided closure asynchronously on the coordinator’s queue and awaits the result.

func performAndWait&lt;T>(() throws -> T) rethrows -> T

Executes the provided closure on the coordinator’s queue and waits for it to finish.

func perform(() -> Void)

Executes the provided closure asynchronously on the coordinator’s queue.

Deprecated

func performAndWait(() -> Void)

Executes the provided closure on the coordinator’s queue and waits for it to finish.

Deprecated

func execute(NSPersistentStoreRequest, with: NSManagedObjectContext) throws -> Any

Executes the specified request on each of the coordinator’s persistent stores.

### Maintaining a record of changes

let NSPersistentHistoryTrackingKey: String

The key you use to enable persistent history tracking.

func currentPersistentHistoryToken(fromStores: [Any]?) -> NSPersistentHistoryToken?

Returns a single persistent history token representing all of the specified stores.

### Integrating with Spotlight

let NSCoreDataCoreSpotlightExporter: String

The key you use to specify your Core Spotlight delegate.

class NSCoreDataCoreSpotlightDelegate

A set of methods that enable integration with Core Spotlight.

Spotlight record keys

The keys for the values that exist in Spotlight’s external record files.

Showcase App Data in Spotlight

Index app data so users can find it by using Spotlight search.

### Getting individual object identifiers

func managedObjectID(forURIRepresentation: URL) -> NSManagedObjectID?

Returns the object identifier for the specified URI representation.

### Responding to changes of the coordinator’s registered stores

static let NSPersistentStoreCoordinatorStoresWillChange: NSNotification.Name

A notification that posts before a coordinator changes its registered stores.

static let NSPersistentStoreCoordinatorStoresDidChange: NSNotification.Name

A notification that the coordinator posts after its registered stores change.

static let NSPersistentStoreCoordinatorWillRemoveStore: NSNotification.Name

A notification that posts before a coordinator removes a store.

Notification keys

The keys you use to retrieve values from a notification’s user info dictionary.

### Deprecated

Deprecated Symbols

Review unsupported symbols and their replacements.

### Instance Methods

func managedObjectID(for: String) -> NSManagedObjectID?

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSLocking
- NSObjectProtocol
- Sendable

## See Also

### Store Coordination

class NSPersistentStore

The abstract base class for all Core Data persistent stores.

class NSPersistentStoreDescription

A description object used to create and load a persistent store.

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

