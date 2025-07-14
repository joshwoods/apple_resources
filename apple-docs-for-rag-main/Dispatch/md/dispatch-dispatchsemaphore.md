

- Dispatch
-  DispatchSemaphore 

Class

# DispatchSemaphore

An object that controls access to a resource across multiple execution contexts through use of a traditional counting semaphore.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
class DispatchSemaphore
```

## Overview

A dispatch semaphore is an efficient implementation of a traditional counting semaphore. Dispatch semaphores call down to the kernel only when the calling thread needs to be blocked. If the calling semaphore does not need to block, no kernel call is made.

You increment a semaphore count by calling the signal() method, and decrement a semaphore count by calling wait() or one of its variants that specifies a timeout.

## Topics

### Creating a Semaphore

init(value: Int)

Creates new counting semaphore with an initial value.

### Signaling the Semaphore

func signal() -> Int

Signals (increments) a semaphore.

### Blocking on the Semaphore

func wait()

Waits for, or decrements, a semaphore.

func wait(timeout: DispatchTime) -> DispatchTimeoutResult

Waits for, or decrements, a semaphore.

func wait(wallTimeout: DispatchWallTime) -> DispatchTimeoutResult

Waits for, or decrements, a semaphore.

## Relationships

### Inherits From

- DispatchObject

### Conforms To

- CVarArg
- Equatable
- Hashable
- NSObjectProtocol
- Sendable

## See Also

### Task Synchronization

Dispatch Semaphore

An object that controls access to a resource across multiple execution contexts through use of a traditional counting semaphore.

Dispatch Barrier

A synchronization point for tasks executing in a concurrent dispatch queue.

