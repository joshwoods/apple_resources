

- Kernel
- IOKit Fundamentals
- Locks
-  IORecursiveLockAlloc 

Function

# IORecursiveLockAlloc

Allocates and initializes an recursive lock.

DriverKitKernelDriverKit 24.4+macOS 10.0+

**DriverKit**

``` source
struct IORecursiveLock * IORecursiveLockAlloc(void);
```

**macOS**

``` source
IORecursiveLock * IORecursiveLockAlloc(void);
```

## Return Value

Pointer to the allocated lock, or zero on failure.

## Discussion

Allocates a recursive lock in general purpose memory, and initializes it. Recursive locks function identically to mutexes but allow one thread to lock more than once, with balanced unlocks. IORecursiveLocks use the global IOKit lock group, IOLockGroup. To simplify kext debugging and lock-heat analysis, consider using lck\_\* locks with a per-driver lock group, as defined in kern/locks.h.

## See Also

### Recursive Locks

IORecursiveLockFree

Frees a recursive lock.

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

