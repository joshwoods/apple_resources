

- Core Data
- NSPersistentStoreCoordinator
-  lock() Deprecated

Instance Method

# lock()

Attempts to acquire a lock.

iOS 3.0–8.0DeprecatediPadOS 3.0–8.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 10.4–10.10DeprecatedvisionOS 1.0–1.0Deprecated

``` source
func lock()
```

Deprecated

Use -performBlockAndWait: instead

## Discussion

This method blocks a thread’s execution until the lock can be acquired. An application protects a critical section of code by requiring a thread to acquire a lock before executing the code. Once the critical section is past, the thread relinquishes the lock by invoking unlock.

## See Also

### Deprecated instance methods

func addPersistentStore(ofType: String, configurationName: String?, at: URL?, options: [AnyHashable : Any]?) throws -> NSPersistentStore

Adds a specific type of persistent store at the provided location.

Deprecated

func destroyPersistentStore(at: URL, ofType: String, options: [AnyHashable : Any]?) throws

Deletes a specific type of persistent store at the provided location.

Deprecated

func importStore(withIdentifier: String?, fromExternalRecordsDirectoryAt: URL, to: URL, options: [AnyHashable : Any]?, ofType: String) throws -> NSPersistentStore

Creates and populates a store with the external records found at a given URL.

Deprecated

func migratePersistentStore(NSPersistentStore, to: URL, options: [AnyHashable : Any]?, withType: String) throws -> NSPersistentStore

Changes the location and, if necessary, the store type of the specified persistent store.

Deprecated

func replacePersistentStore(at: URL, destinationOptions: [AnyHashable : Any]?, withPersistentStoreFrom: URL, sourceOptions: [AnyHashable : Any]?, ofType: String) throws

Replaces one persistent store with another.

Deprecated

func tryLock() -> Bool

Attempts to acquire a lock.

Deprecated

func unlock()

Relinquishes a previously acquired lock.

Deprecated

func perform(() -> Void)

Executes the provided closure asynchronously on the coordinator’s queue.

Deprecated

func performAndWait(() -> Void)

Executes the provided closure on the coordinator’s queue and waits for it to finish.

Deprecated

