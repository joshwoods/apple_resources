

- Kernel
- IOKit Fundamentals
- Locks
-  IOTryLock 

Function

# IOTryLock

macOS 10.0+

``` source
boolean_t IOTryLock(IOLock *lock);
```

## See Also

### Mutexes

IOLockAlloc

Allocates and initializes a mutex.

IOLockInitWithState

IOLockFree

Frees a mutex.

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

IOLockSleepDeadline

IOLockGetMachLock

Accessor to a Mach mutex.

