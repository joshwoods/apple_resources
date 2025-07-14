

- Kernel
- IOKit Fundamentals
- Locks
-  IOLockFree 

Function

# IOLockFree

Frees a mutex.

DriverKitKernelDriverKit 24.4+macOS 10.0+

**DriverKit**

``` source
void IOLockFree(struct IOLock *lock);
```

**macOS**

``` source
void IOLockFree(IOLock *lock);
```

## Parameters 

`lock`  

Pointer to the allocated lock.

## Discussion

Frees a lock allocated with IOLockAlloc. Mutex should be unlocked with no waiters.

## See Also

### Mutexes

IOLockAlloc

Allocates and initializes a mutex.

IOLockInitWithState

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

