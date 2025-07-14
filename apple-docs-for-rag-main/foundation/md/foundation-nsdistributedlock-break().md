

- Foundation
- NSDistributedLock
-  break() 

Instance Method

# break()

Forces the lock to be relinquished.

Mac Catalyst 13.0+macOS 10.0+

``` source
func `break`()
```

## Discussion

This method always succeeds unless the lock has been damaged. If another process has already unlocked or broken the lock, this method has no effect. You should generally use unlock() rather than break() to relinquish a lock.

Warning

Because `breakLock` can release another process’s lock, it should be used with great caution.

Even if you break a lock, there’s no guarantee that you will then be able to acquire the lock—another process might get it before your try() is invoked.

Raises an `NSGenericException` if the lock could not be removed.

## See Also

### Relinquishing a Lock

func unlock()

Relinquishes the receiver.

