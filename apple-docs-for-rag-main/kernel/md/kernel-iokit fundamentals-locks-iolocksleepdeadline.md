

- Kernel
- IOKit Fundamentals
- Locks
-  IOLockSleepDeadline 

Function

# IOLockSleepDeadline

macOS 10.2+

``` source
int IOLockSleepDeadline(IOLock *lock, void *event, AbsoluteTime deadline, UInt32 interType);
```

## See Also

### Mutexes

IOLockAlloc

Allocates and initializes a mutex.

IOLockInitWithState

IOLockFree

Frees a mutex.

IOTryLock

IOTakeLock

IOLockLock

Lock a mutex.

IOUnlock

IOLockTryLock

Attempt to lock a mutex.

IOLockUnlock

Unlock a mutex.

IOLockWakeup

IOLockSleep

Sleep with mutex unlock and relock

IOLockGetMachLock

Accessor to a Mach mutex.

