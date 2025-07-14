

- os
- OSAllocatedUnfairLock
-  precondition(\_:) 

Instance Method

# precondition(\_:)

Asserts if the lock object fails to meet specified ownership requirements.

iOS 16.0+iPadOS 16.0+Mac CatalystmacOS 13.0+tvOS 16.0+visionOSwatchOS 9.0+

``` source
func precondition(_ condition: OSAllocatedUnfairLock.Ownership)
```

## Parameters 

`condition`  

The ownership status to check.

## Discussion

Call this function to ensure the ownership state of the lock is what your code requires. For example, if you call this function and pass OSAllocatedUnfairLock.Ownership.owner, the app terminates if the object is locked, but the calling code doesn’t own the lock. Similarly, if you call it and pass OSAllocatedUnfairLock.Ownership.notOwner, the app terminates if the calling code doesn’t own the lock, or if the object isn’t locked.

## See Also

### Determining lock ownership

enum Ownership

An enumeration that represents the ownership status of an unfair lock.

