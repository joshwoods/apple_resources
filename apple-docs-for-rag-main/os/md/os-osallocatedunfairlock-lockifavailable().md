

- os
- OSAllocatedUnfairLock
-  lockIfAvailable() 

Instance Method

# lockIfAvailable()

Attempts to acquire a lock.

iOS 16.0+iPadOS 16.0+Mac CatalystmacOS 13.0+tvOS 16.0+visionOSwatchOS 9.0+

``` source
func lockIfAvailable() -> Bool
```

Available when `State` is `()`.

## Return Value

true if successful; otherwise, false.

## See Also

### Using locks

func lock()

Acquires a lock.

func unlock()

Ends the lock.

