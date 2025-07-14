

- Kernel
- IOKit Fundamentals
- Locks
-  IOLockInitWithState 

Function

# IOLockInitWithState

macOS 10.0+

``` source
void IOLockInitWithState(IOLock *lock, IOLockState state);
```

## See Also

### Mutexes

IOLockAlloc

Allocates and initializes a mutex.

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

IOLockSleepDeadline

IOLockGetMachLock

Accessor to a Mach mutex.

