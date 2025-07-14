

- Kernel
- IOKit Fundamentals
- Locks
-  IOLockTryLock 

Function

# IOLockTryLock

Attempt to lock a mutex.

DriverKitKernelDriverKit 24.4+macOS 10.0+

**DriverKit**

``` source
bool IOLockTryLock(struct IOLock *lock);
```

**macOS**

``` source
boolean_t IOLockTryLock(IOLock *lock);
```

## Parameters 

`lock`  

Pointer to the allocated lock.

## Discussion

Lock the mutex if it is currently unlocked, and return true. If the lock is held by any thread, return false.

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

IOLockUnlock

Unlock a mutex.

IOLockWakeup

IOLockSleep

Sleep with mutex unlock and relock

IOLockSleepDeadline

IOLockGetMachLock

Accessor to a Mach mutex.

