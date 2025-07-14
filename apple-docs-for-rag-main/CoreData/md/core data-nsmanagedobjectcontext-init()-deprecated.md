

- Core Data
- NSManagedObjectContext
-  init() Deprecated

Initializer

# init()

iOS 3.0–9.0DeprecatediPadOS 3.0–9.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 10.4–10.11DeprecatedtvOSDeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 2.0–2.0Deprecated

``` source
convenience init()
```

Deprecated

Use -initWithConcurrencyType: instead

## See Also

### Deprecated instance methods

init(concurrencyType: NSManagedObjectContextConcurrencyType)

Creates a context that uses the specified concurrency type.

Deprecated

func lock()

Attempts to acquire a lock on the context.

Deprecated

func tryLock() -> Bool

Attempts to acquire a lock.

Deprecated

func unlock()

Relinquishes a previously acquired lock.

Deprecated

