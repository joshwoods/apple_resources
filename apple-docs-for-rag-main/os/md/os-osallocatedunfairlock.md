

- os
-  OSAllocatedUnfairLock 

Structure

# OSAllocatedUnfairLock

A structure that creates an unfair lock.

iOS 16.0+iPadOS 16.0+Mac CatalystmacOS 13.0+tvOS 16.0+visionOSwatchOS 9.0+

``` source
@frozen
struct OSAllocatedUnfairLock
```

## Overview

Unfair locks are low-level locks that block efficiently on contention. They’re useful for protecting code that loads stored resources. However, it’s unsafe to use os_unfair_lock from Swift because it’s a value type and, therefore, doesn’t have a stable memory address. That means when you call os_unfair_lock_lock or os_unfair_lock_unlock and pass a lock object using the `&` operator, the system may lock or unlock the wrong object.

Instead, use OSAllocatedUnfairLock, which avoids that pitfall because it doesn’t function as a value type, despite being a structure. All copied instances of an OSAllocatedUnfairLock control the same underlying lock allocation.

Important

If you’ve existing Swift code that uses os_unfair_lock, change it to use OSAllocatedUnfairLock to ensure correct locking behavior.

To create a lock that protects operation state, create an enumeration that contains the possible states, then create a lock object, passing the initial state. Here’s an example of what that looks like for an asset load operation:

```
enum MyState {
    case idle
    case loading
    case complete(MyAsset)
    case error(Error)
}
let protectedState = OSAllocatedUnfairLock(initialState: MyState.idle)
```

Storing the state inside the lock helps track what the lock is protecting, and provides a way to safely access the state. To begin using the lock, call `withLock(_:)` or `withLockIfAvailable(_:)`, passing a closure that contains the code for the lock to protect, like in the following example:

```
func myLoadMethod() {
    protectedState.withLock { state in
        state = .loading
    }
    var (resource, error) = loadMyResources()
    if resource != nil {
        protectedState.withLock { state in
            state = .complete(resource)
        }
    } else {
        protectedState.withLock { state in
            state = .error(error!)
        }
    }
}
```

To protect an operation with an externally defined state or no state, create a lock object without specifying an initial state. Nonscoped locking is more flexible, but offers no assistance in tracking the state of the operation the lock protects. To use a nonscoped lock, use `withLock(_:)` or `withLockIfAvailable(_:)`.

```
let myLock = OSAllocatedUnfairLock()
myLock.withLock {
    // Code that needs protection.
}
```

You can also use OSAllocatedUnfairLock with the more traditional lock/unlock approach by calling lock() before executing code that needs protection, and unlock() upon completion, like this:

```
myLock.lock()
// Code that needs protection.
myLock.unlock()
```

When using this approach, you must call unlock() from the same thread you use to call lock(). Because of this, it’s unsafe to use this approach across an `await` suspension point. When using a lock with asynchronous code, lock using a closure or, even better, consider using an Actor.

Warning

OSAllocatedUnfairLock isn’t a recursive lock. Attempting to lock an object more than once from the same thread without unlocking in between triggers a runtime exception.

## Topics

### Creating a lock object

init()

Creates a lock object that doesn’t protect state data.

init(initialState: State)

Creates a lock object that maintains and protects state data.

### Using locks

func lock()

Acquires a lock.

func lockIfAvailable() -> Bool

Attempts to acquire a lock.

func unlock()

Ends the lock.

### Determining lock ownership

enum Ownership

An enumeration that represents the ownership status of an unfair lock.

func precondition(OSAllocatedUnfairLock&lt;State>.Ownership)

Asserts if the lock object fails to meet specified ownership requirements.

### Initializers

init(uncheckedState: State)

### Instance Methods

func lock(flags: OSAllocatedUnfairLockFlags)

func withLock&lt;R>((inout State) throws -> R) rethrows -> R

func withLock&lt;R>(() throws -> R) rethrows -> R

func withLock&lt;R>(flags: OSAllocatedUnfairLockFlags, (inout State) throws -> R) rethrows -> R

func withLock&lt;R>(flags: OSAllocatedUnfairLockFlags, () throws -> R) rethrows -> R

func withLockIfAvailable&lt;R>(() throws -> R) rethrows -> R?

func withLockIfAvailable&lt;R>((inout State) throws -> R) rethrows -> R?

func withLockIfAvailableUnchecked&lt;R>((inout State) throws -> R) rethrows -> R?

func withLockIfAvailableUnchecked&lt;R>(() throws -> R) rethrows -> R?

func withLockUnchecked&lt;R>((inout State) throws -> R) rethrows -> R

func withLockUnchecked&lt;R>(() throws -> R) rethrows -> R

func withLockUnchecked&lt;R>(flags: OSAllocatedUnfairLockFlags, (inout State) throws -> R) rethrows -> R

func withLockUnchecked&lt;R>(flags: OSAllocatedUnfairLockFlags, () throws -> R) rethrows -> R

## Relationships

### Conforms To

- Sendable

## See Also

### Swift Wrappers

struct OSAllocatedUnfairLockFlags

