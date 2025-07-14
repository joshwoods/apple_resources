

- Kernel
- IOKit Fundamentals
- Locks
-  IORecursiveLockGetMachLock 

Function

# IORecursiveLockGetMachLock

Accessor to a Mach mutex.

macOS 10.4+

``` source
lck_mtx_t * IORecursiveLockGetMachLock(IORecursiveLock *lock);
```

## Parameters 

`lock`  

Pointer to the allocated lock.

## Discussion

Accessor to the Mach mutex.

## See Also

### Recursive Locks

IORecursiveLockAlloc

Allocates and initializes an recursive lock.

IORecursiveLockFree

Frees a recursive lock.

IORecursiveLockHaveLock

Check if a recursive lock is held by the calling thread.

IORecursiveLockLock

Lock a recursive lock.

IORecursiveLockSleep

IORecursiveLockSleepDeadline

IORecursiveLockTryLock

Attempt to lock a recursive lock.

IORecursiveLockUnlock

Unlock a recursive lock.

IORecursiveLockWakeup

