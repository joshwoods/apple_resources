

- Open Directory
- ODQuery
-  operationQueue 

Instance Property

# operationQueue

The queue on which asynchronous results are delivered to the delegate.

Mac CatalystmacOS 10.6+

``` source
var operationQueue: OperationQueue! { get set }
```

## See Also

### Managing Asynchronous Queries

var delegate: (any ODQueryDelegate)!

The query’s delegate.

func schedule(in: RunLoop!, forMode: String!)

Retrieves results from a query asynchronously by scheduling the query in a run loop.

func remove(from: RunLoop!, forMode: String!)

Removes the query from a specified run loop.

func synchronize()

Restarts a query, disposing of any results it has obtained.

