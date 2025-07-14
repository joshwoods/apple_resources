

- Dispatch
-  Dispatch Semaphore 

API Collection

# Dispatch Semaphore

An object that controls access to a resource across multiple execution contexts through use of a traditional counting semaphore.

## Overview

A dispatch semaphore is an efficient implementation of a traditional counting semaphore. Dispatch semaphores call down to the kernel only when the calling thread needs to be blocked. If the calling semaphore does not need to block, no kernel call is made.

You increment a semaphore count by calling the signal() method, and decrement a semaphore count by calling dispatch_semaphore_wait or one of its variants that specifies a timeout.

## Topics

### Creating a Semaphore

init(value: Int)

Creates new counting semaphore with an initial value.

typealias dispatch_semaphore_t

A dispatch semaphore object.

## See Also

### Task Synchronization

class DispatchSemaphore

An object that controls access to a resource across multiple execution contexts through use of a traditional counting semaphore.

Dispatch Barrier

A synchronization point for tasks executing in a concurrent dispatch queue.

