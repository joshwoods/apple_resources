

- Kernel
- IOKit Fundamentals
- Locks
-  IORecursiveLockHaveLock 

Function

# IORecursiveLockHaveLock

Check if a recursive lock is held by the calling thread.

DriverKitKernelDriverKit 24.4+macOS 10.0+

**DriverKit**

``` source
bool IORecursiveLockHaveLock(struct IORecursiveLock *lock);
```

**macOS**

``` source
boolean_t IORecursiveLockHaveLock(const IORecursiveLock *lock);
```

## Parameters 

`lock`  

Pointer to the allocated lock.

## Return Value

True if the calling thread holds the lock otherwise false.

## Discussion

If the lock is held by the calling thread, return true, otherwise the lock is unlocked, or held by another thread and false is returned.

## See Also

### Recursive Locks

IORecursiveLockAlloc

Allocates and initializes an recursive lock.

IORecursiveLockFree

Frees a recursive lock.

IORecursiveLockGetMachLock

Accessor to a Mach mutex.

IORecursiveLockLock

Lock a recursive lock.

IORecursiveLockSleep

IORecursiveLockSleepDeadline

IORecursiveLockTryLock

Attempt to lock a recursive lock.

IORecursiveLockUnlock

Unlock a recursive lock.

IORecursiveLockWakeup

