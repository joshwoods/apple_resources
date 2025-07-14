

- Kernel
- IOKit Fundamentals
- Locks
-  IOLockUnlock 

Function

# IOLockUnlock

Unlock a mutex.

DriverKitKernelDriverKit 24.4+macOS 10.0+

**DriverKit**

``` source
void IOLockUnlock(struct IOLock *lock);
```

**macOS**

``` source
void IOLockUnlock(IOLock *lock);
```

## Parameters 

`lock`  

Pointer to the allocated lock.

## Discussion

Unlock the mutex and wake any blocked waiters. Results are undefined if the caller has not locked the mutex. This function may block and so should not be called from interrupt level or while a spin lock is held.

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

IOLockWakeup

IOLockSleep

Sleep with mutex unlock and relock

IOLockSleepDeadline

IOLockGetMachLock

Accessor to a Mach mutex.

