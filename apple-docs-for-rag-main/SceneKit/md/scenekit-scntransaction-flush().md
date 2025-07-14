

- SceneKit
- SCNTransaction
-  flush() 

Type Method

# flush()

Applies all changes from the current automatic transaction.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
class func flush()
```

## Discussion

SceneKit automatically calls this method at the end of each pass through the run loop, regardless of the run loop mode. If your app does not have a run loop, you must call this method explicitly.

If the current transaction has any nested transactions that are still animating, SceneKit waits to commit the current transaction’s changes until those transactions complete.

Note

If possible, avoid calling flush() explicitly. By allowing flush() to execute during the run loop, your app achieves better performance, atomic screen updates are preserved, and transactions and animations that work from transaction to transaction continue to function.

## See Also

### Creating and Committing Transactions

class func begin()

Begins a new transaction for the current thread.

class func commit()

Commits all changes made during the current transaction.

