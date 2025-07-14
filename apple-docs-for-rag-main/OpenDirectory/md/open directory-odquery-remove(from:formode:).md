

- Open Directory
- ODQuery
-  remove(from:forMode:) 

Instance Method

# remove(from:forMode:)

Removes the query from a specified run loop.

Mac CatalystmacOS 10.6+

``` source
func remove(
    from inRunLoop: RunLoop!,
    forMode inMode: String!
)
```

## Parameters 

`inRunLoop`  

The run loop.

`inMode`  

The mode to remove the query from.

## See Also

### Managing Asynchronous Queries

var delegate: (any ODQueryDelegate)!

The query’s delegate.

var operationQueue: OperationQueue!

The queue on which asynchronous results are delivered to the delegate.

func schedule(in: RunLoop!, forMode: String!)

Retrieves results from a query asynchronously by scheduling the query in a run loop.

func synchronize()

Restarts a query, disposing of any results it has obtained.

