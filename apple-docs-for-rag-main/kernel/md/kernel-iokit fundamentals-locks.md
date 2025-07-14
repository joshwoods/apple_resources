

- Kernel
- IOKit Fundamentals
-  Locks 

API Collection

# Locks

## Topics

### Simple Locks

IOSimpleLockAlloc

Allocates and initializes a spin lock.

IOSimpleLockInit

Initialize a spin lock.

IOSimpleLockDestroy

IOSimpleLockFree

Frees a spin lock.

IOSimpleLockGetMachLock

Accessor to a Mach spin lock.

IOSimpleLockLock

Lock a spin lock.

IOSimpleLockLockDisableInterrupt

Lock a spin lock.

IOSimpleLockTryLock

Attempt to lock a spin lock.

IOSimpleLockUnlock

Unlock a spin lock.

IOSimpleLockUnlockEnableInterrupt

Unlock a spin lock, and restore interrupt state.

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

IOLockSleep

Sleep with mutex unlock and relock

IOLockSleepDeadline

IOLockGetMachLock

Accessor to a Mach mutex.

### Read/Write Locks

IORWLockAlloc

Allocates and initializes a read/write lock.

IORWLockFree

Frees a read/write lock.

IORWLockGetMachLock

Accessor to a Mach read/write lock.

IORWLockRead

Lock a read/write lock for read.

IORWLockUnlock

Unlock a read/write lock.

IORWLockWrite

Lock a read/write lock for write.

IORWUnlock

IOWriteLock

IOReadLock

### Recursive Locks

IORecursiveLockAlloc

Allocates and initializes an recursive lock.

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

### Condition Lock

IOConditionLock

## See Also

### Resources

Memory

Allocate, map, free, and manage memory in the kernel.

Workflow and Control

Data Types

Create strings, numbers, collections, data objects, and the other standard types employed by drivers and kernel extensions.

