

- Open Directory
- ODQuery
-  synchronize() 

Instance Method

# synchronize()

Restarts a query, disposing of any results it has obtained.

Mac CatalystmacOS 10.6+

``` source
func synchronize()
```

## Discussion

If the query was originally scheduled in a run loop with schedule(in:forMode:), the delegate is called with `inResults` set to `nil`, `[inError code]` set to `kODErrorQuerySynchronize`, and `[inError domain]` set to `kODErrorDomainFramework`.

## See Also

### Managing Asynchronous Queries

var delegate: (any ODQueryDelegate)!

The query’s delegate.

var operationQueue: OperationQueue!

The queue on which asynchronous results are delivered to the delegate.

func schedule(in: RunLoop!, forMode: String!)

Retrieves results from a query asynchronously by scheduling the query in a run loop.

func remove(from: RunLoop!, forMode: String!)

Removes the query from a specified run loop.

