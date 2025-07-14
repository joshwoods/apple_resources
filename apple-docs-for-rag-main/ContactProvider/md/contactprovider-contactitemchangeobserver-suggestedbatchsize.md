

- ContactProvider
- ContactItemChangeObserver
-  suggestedBatchSize 

Instance Property

# suggestedBatchSize

Retrieves the suggested number of changed contact items to include in a batch.

iOS 18.0+iPadOS 18.0+

``` source
var suggestedBatchSize: Int { get }
```

**Required**

## Discussion

This value is a suggested upper limit for the number of contact items you can pass in the aggregate calls to didUpdate(_:) and didDelete(_:). Exceeding this limit may result in memory issues.

