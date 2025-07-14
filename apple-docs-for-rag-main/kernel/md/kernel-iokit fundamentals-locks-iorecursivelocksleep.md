

- Kernel
- IOKit Fundamentals
- Locks
-  IORecursiveLockSleep 

Function

# IORecursiveLockSleep

macOS 10.0+

``` source
int IORecursiveLockSleep(IORecursiveLock *_lock, void *event, UInt32 interType);
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

IORecursiveLockSleepDeadline

IORecursiveLockTryLock

Attempt to lock a recursive lock.

IORecursiveLockUnlock

Unlock a recursive lock.

IORecursiveLockWakeup

