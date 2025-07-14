

- os
-  Synchronization 

API Collection

# Synchronization

Access low-level synchronization mechanisms to control state across threads.

## Overview

Note

When possible, use higher-level synchronization primitives such as `pthread`, Grand Central Dispatch, or Swift’s concurrency features to control access to state across different threads. For more information, see Updating an App to Use Swift Concurrency.

## Topics

### Swift Wrappers

struct OSAllocatedUnfairLock

A structure that creates an unfair lock.

struct OSAllocatedUnfairLockFlags

