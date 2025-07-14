

- Core Animation
- CATransaction
-  begin() 

Type Method

# begin()

Begin a new transaction for the current thread.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+

``` source
class func begin()
```

## Discussion

The transaction is nested within the thread’s current transaction, if there is one.

## See Also

### Related Documentation

Core Animation Programming Guide

### Creating and Committing Transactions

class func commit()

Commit all changes made during the current transaction.

class func flush()

Flushes any extant implicit transaction.

