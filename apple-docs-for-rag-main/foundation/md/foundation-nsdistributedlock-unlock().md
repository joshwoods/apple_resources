

- Foundation
- NSDistributedLock
-  unlock() 

Instance Method

# unlock()

Relinquishes the receiver.

Mac Catalyst 13.0+macOS 10.0+

``` source
func unlock()
```

## Discussion

You should generally use the unlock() method rather than break() to release a lock.

An `NSGenericException` is raised if the receiver doesn’t already exist.

## See Also

### Relinquishing a Lock

func `break`()

Forces the lock to be relinquished.

