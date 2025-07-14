

- SceneKit
- SCNTransaction
-  commit() 

Type Method

# commit()

Commits all changes made during the current transaction.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
class func commit()
```

## Discussion

If there is no current transaction, this method has no effect.

## See Also

### Creating and Committing Transactions

class func begin()

Begins a new transaction for the current thread.

class func flush()

Applies all changes from the current automatic transaction.

