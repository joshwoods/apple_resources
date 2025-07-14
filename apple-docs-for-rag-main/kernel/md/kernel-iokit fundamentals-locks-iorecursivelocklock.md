

- Kernel
- IOKit Fundamentals
- Locks
-  IORecursiveLockLock 

Function

# IORecursiveLockLock

Lock a recursive lock.

DriverKitKernelDriverKit 24.4+macOS 10.0+

**DriverKit**

``` source
void IORecursiveLockLock(struct IORecursiveLock *lock);
```

**macOS**

``` source
void IORecursiveLockLock(IORecursiveLock *lock);
```

## Parameters 

`lock`  

Pointer to the allocated lock.

## Discussion

Lock the recursive lock. If the lock is held by another thread, block waiting for its unlock. This function may block and so should not be called from interrupt level or while a spin lock is held. The lock may be taken recursively by the same thread, with a balanced number of calls to IORecursiveLockUnlock.

## See Also

### Recursive Locks

IORecursiveLockAlloc

Allocates and initializes an recursive lock.

IORecursiveLockFree

Frees a recursive lock.

IORecursiveLockGetMachLock

Accessor to a Mach mutex.

IORecursiveLockHaveLock

Check if a recursive lock is held by the calling thread.

IORecursiveLockSleep

IORecursiveLockSleepDeadline

IORecursiveLockTryLock

Attempt to lock a recursive lock.

IORecursiveLockUnlock

Unlock a recursive lock.

IORecursiveLockWakeup

