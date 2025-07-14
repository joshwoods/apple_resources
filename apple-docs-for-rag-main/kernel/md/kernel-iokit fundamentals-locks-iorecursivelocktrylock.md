

- Kernel
- IOKit Fundamentals
- Locks
-  IORecursiveLockTryLock 

Function

# IORecursiveLockTryLock

Attempt to lock a recursive lock.

DriverKitKernelDriverKit 24.4+macOS 10.0+

**DriverKit**

``` source
bool IORecursiveLockTryLock(struct IORecursiveLock *lock);
```

**macOS**

``` source
boolean_t IORecursiveLockTryLock(IORecursiveLock *lock);
```

## Parameters 

`lock`  

Pointer to the allocated lock.

## Return Value

True if the lock is now locked by the caller, otherwise false.

## Discussion

Lock the lock if it is currently unlocked, or held by the calling thread, and return true. If the lock is held by another thread, return false. Successful calls to IORecursiveLockTryLock should be balanced with calls to IORecursiveLockUnlock.

## See Also

### Recursive Locks

IORecursiveLockAlloc

Allocates and initializes an recursive lock.

IORecursiveLockFree

Frees a recursive lock.

IORecursiveLockGetMachLock

Accessor to a Mach mutex.

IORecursiveLockHaveLock

Check if a recursive lock is held by the calling thread.

IORecursiveLockLock

Lock a recursive lock.

IORecursiveLockSleep

IORecursiveLockSleepDeadline

IORecursiveLockUnlock

Unlock a recursive lock.

IORecursiveLockWakeup

