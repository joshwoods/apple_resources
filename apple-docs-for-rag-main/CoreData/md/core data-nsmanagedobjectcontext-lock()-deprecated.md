

- Core Data
- NSManagedObjectContext
-  lock() Deprecated

Instance Method

# lock()

Attempts to acquire a lock on the context.

iOS 3.0–8.0DeprecatediPadOS 3.0–8.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 10.4–10.10DeprecatedvisionOS 1.0–1.0Deprecated

``` source
func lock()
```

Deprecated

Use a queue style context and -performBlockAndWait: instead

## Discussion

This method blocks a thread’s execution until the lock can be acquired. An application protects a critical section of code by requiring a thread to acquire a lock before executing the code. Once the critical section is past, the thread relinquishes the lock by invoking unlock().

Sending this message to a managed object context helps the framework to understand the scope of a transaction in a multi-threaded environment. It is preferable to use the `NSManagedObjectContext`’s implementation of `NSLocking` instead using of a separate mutex object.

If you lock (or successfully `tryLock`) a managed object context, the thread in which the lock call is made must keep a strong reference to the context until it invokes unlock, otherwise if the context is deallocated this will result in deadlock.

## See Also

### Deprecated instance methods

init(concurrencyType: NSManagedObjectContextConcurrencyType)

Creates a context that uses the specified concurrency type.

Deprecated

convenience init()Deprecated

func tryLock() -> Bool

Attempts to acquire a lock.

Deprecated

func unlock()

Relinquishes a previously acquired lock.

Deprecated

