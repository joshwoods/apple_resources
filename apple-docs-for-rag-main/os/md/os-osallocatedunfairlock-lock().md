

- os
- OSAllocatedUnfairLock
-  lock() 

Instance Method

# lock()

Acquires a lock.

iOS 16.0+iPadOS 16.0+Mac CatalystmacOS 13.0+tvOS 16.0+visionOSwatchOS 9.0+

``` source
func lock()
```

Available when `State` is `()`.

## See Also

### Using locks

func lockIfAvailable() -> Bool

Attempts to acquire a lock.

func unlock()

Ends the lock.

