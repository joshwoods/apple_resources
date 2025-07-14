

- SceneKit
- SCNTransaction
-  begin() 

Type Method

# begin()

Begins a new transaction for the current thread.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
class func begin()
```

## Discussion

The new transaction is nested within the thread’s current transaction, if there is one.

The first time you modify the scene graph during a pass through the run loop, SceneKit automatically creates a transaction and makes it the current transaction. (SceneKit commits that transaction when the next iteration of the run loops begins.) If you call this method to create a custom transaction before modifying the scene graph, your custom transaction becomes the current transaction.

## See Also

### Creating and Committing Transactions

class func commit()

Commits all changes made during the current transaction.

class func flush()

Applies all changes from the current automatic transaction.

