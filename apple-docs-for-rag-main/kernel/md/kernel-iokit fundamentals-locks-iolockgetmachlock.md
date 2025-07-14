

- Kernel
- IOKit Fundamentals
- Locks
-  IOLockGetMachLock 

Function

# IOLockGetMachLock

Accessor to a Mach mutex.

macOS 10.4+

``` source
lck_mtx_t * IOLockGetMachLock(IOLock *lock);
```

## Parameters 

`lock`  

Pointer to the allocated lock.

## Discussion

Accessor to the Mach mutex.

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

IOLockSleepDeadline

