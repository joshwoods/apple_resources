

- Kernel
- IOKit Fundamentals
- Locks
-  IOLockSleep 

Function

# IOLockSleep

Sleep with mutex unlock and relock

macOS 10.2+

``` source
int IOLockSleep(IOLock *lock, void *event, UInt32 interType);
```

## Parameters 

`lock`  

Pointer to the locked lock.

`event`  

The event to sleep on.

`interType`  

How can the sleep be interrupted.

## Return Value

The wait-result value indicating how the thread was awakened.

## Discussion

Prepare to sleep,unlock the mutex, and re-acquire it on wakeup. Results are undefined if the caller has not locked the mutex. This function may block and so should not be called from interrupt level or while a spin lock is held.

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

IOLockSleepDeadline

IOLockGetMachLock

Accessor to a Mach mutex.

