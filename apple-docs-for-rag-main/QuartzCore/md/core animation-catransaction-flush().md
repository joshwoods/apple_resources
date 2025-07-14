

- Core Animation
- CATransaction
-  flush() 

Type Method

# flush()

Flushes any extant implicit transaction.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+

``` source
class func flush()
```

## Discussion

Delays the commit until any nested explicit transactions have completed.

Flush is typically called automatically at the end of the current runloop, regardless of the runloop mode. If your application does not have a runloop, you must call this method explicitly.

However, you should attempt to avoid calling `flush` explicitly. By allowing `flush` to execute during the runloop your application will achieve better performance, atomic screen updates will be preserved, and transactions and animations that work from transaction to transaction will continue to function.

## See Also

### Creating and Committing Transactions

class func begin()

Begin a new transaction for the current thread.

class func commit()

Commit all changes made during the current transaction.

