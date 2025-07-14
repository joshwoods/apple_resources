

- Kernel
- IOKit Fundamentals
- Locks
-  IORecursiveLockWakeup 

Function

# IORecursiveLockWakeup

macOS 10.0+

``` source
void IORecursiveLockWakeup(IORecursiveLock *_lock, void *event, bool oneThread);
```

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

IORecursiveLockTryLock

Attempt to lock a recursive lock.

IORecursiveLockUnlock

Unlock a recursive lock.

