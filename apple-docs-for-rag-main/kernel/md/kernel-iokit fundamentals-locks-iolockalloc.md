

- Kernel
- IOKit Fundamentals
- Locks
-  IOLockAlloc 

Function

# IOLockAlloc

Allocates and initializes a mutex.

DriverKitKernelDriverKit 24.4+macOS 10.0+

**DriverKit**

``` source
struct IOLock * IOLockAlloc(void);
```

**macOS**

``` source
IOLock * IOLockAlloc(void);
```

## Return Value

Pointer to the allocated lock, or zero on failure.

## Discussion

Allocates a mutex in general purpose memory, and initializes it. Mutexes are general purpose blocking mutual exclusion locks, supplied by libkern/locks.h. This function may block and so should not be called from interrupt level or while a spin lock is held. IOLocks use the global IOKit lock group, IOLockGroup. To simplify kext debugging and lock-heat analysis, consider using lck\_\* locks with a per-driver lock group, as defined in kern/locks.h.

## See Also

### Mutexes

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

IOLockGetMachLock

Accessor to a Mach mutex.

