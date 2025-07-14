

- Kernel
- IOKit Fundamentals
- Locks
-  IOLockLock 

Function

# IOLockLock

Lock a mutex.

DriverKitKernelDriverKit 24.4+macOS 10.0+

**DriverKit**

``` source
void IOLockLock(struct IOLock *lock);
```

**macOS**

``` source
void IOLockLock(IOLock *lock);
```

## Parameters 

`lock`  

Pointer to the allocated lock.

## Discussion

Lock the mutex. If the lock is held by any thread, block waiting for its unlock. This function may block and so should not be called from interrupt level or while a spin lock is held. Locking the mutex recursively from one thread will result in deadlock.

## See Also

### Mutexes

IOLockAlloc

Allocates and initializes a mutex.

IOLockInitWithState

IOLockFree

Frees a mutex.

IOTryLock

IOTakeLock

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

