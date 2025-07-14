

- Core Data
- NSManagedObjectContext
-  unlock() Deprecated

Instance Method

# unlock()

Relinquishes a previously acquired lock.

iOS 3.0–8.0DeprecatediPadOS 3.0–8.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 10.4–10.10DeprecatedvisionOS 1.0–1.0Deprecated

``` source
func unlock()
```

Deprecated

Use a queue style context and -performBlockAndWait: instead

## See Also

### Deprecated instance methods

init(concurrencyType: NSManagedObjectContextConcurrencyType)

Creates a context that uses the specified concurrency type.

Deprecated

convenience init()Deprecated

func lock()

Attempts to acquire a lock on the context.

Deprecated

func tryLock() -> Bool

Attempts to acquire a lock.

Deprecated

