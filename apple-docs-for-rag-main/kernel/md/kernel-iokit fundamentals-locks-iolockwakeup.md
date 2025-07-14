

- Kernel
- IOKit Fundamentals
- Locks
-  IOLockWakeup 

Function

# IOLockWakeup

macOS 10.2+

``` source
void IOLockWakeup(IOLock *lock, void *event, bool oneThread);
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

IOLockSleep

Sleep with mutex unlock and relock

IOLockSleepDeadline

IOLockGetMachLock

Accessor to a Mach mutex.

