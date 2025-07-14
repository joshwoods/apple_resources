

- Kernel
- IOKit Fundamentals
- Locks
-  IORecursiveLockFree 

Function

# IORecursiveLockFree

Frees a recursive lock.

DriverKitKernelDriverKit 24.4+macOS 10.0+

**DriverKit**

``` source
void IORecursiveLockFree(struct IORecursiveLock *lock);
```

**macOS**

``` source
void IORecursiveLockFree(IORecursiveLock *lock);
```

## Parameters 

`lock`  

Pointer to the allocated lock.

## Discussion

Frees a lock allocated with IORecursiveLockAlloc. Lock should be unlocked with no waiters.

## See Also

### Recursive Locks

IORecursiveLockAlloc

Allocates and initializes an recursive lock.

IORecursiveLockGetMachLock

Accessor to a Mach mutex.

IORecursiveLockHaveLock

Check if a recursive lock is held by the calling thread.

IORecursiveLockLock

Lock a recursive lock.

IORecursiveLockSleep

IORecursiveLockSleepDeadline

IORecursiveLockTryLock

Attempt to lock a recursive lock.

IORecursiveLockUnlock

Unlock a recursive lock.

IORecursiveLockWakeup

