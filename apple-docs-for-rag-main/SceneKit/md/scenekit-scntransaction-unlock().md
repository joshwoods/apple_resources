

- SceneKit
- SCNTransaction
-  unlock() 

Type Method

# unlock()

Relinquishes a previously acquired transaction lock.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
class func unlock()
```

## Discussion

See the lock() method for more details on transaction locking.

## See Also

### Managing Concurrency

class func lock()

Attempts to acquire a recursive spinlock to ensure the validity of values you retrieve during the transaction.

