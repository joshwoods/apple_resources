

- Kernel
- IOKit Fundamentals
- Locks
-  IORecursiveLockSleepDeadline 

Function

# IORecursiveLockSleepDeadline

macOS 10.6+

``` source
int IORecursiveLockSleepDeadline(IORecursiveLock *_lock, void *event, AbsoluteTime deadline, UInt32 interType);
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

IORecursiveLockTryLock

Attempt to lock a recursive lock.

IORecursiveLockUnlock

Unlock a recursive lock.

IORecursiveLockWakeup

