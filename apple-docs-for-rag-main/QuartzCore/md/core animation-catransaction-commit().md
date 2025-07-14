

- Core Animation
- CATransaction
-  commit() 

Type Method

# commit()

Commit all changes made during the current transaction.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+

``` source
class func commit()
```

## Discussion

Raises an exception if no current transaction exists.

## See Also

### Creating and Committing Transactions

class func begin()

Begin a new transaction for the current thread.

class func flush()

Flushes any extant implicit transaction.

