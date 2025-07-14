

- Open Directory
- ODQuery
-  schedule(in:forMode:) 

Instance Method

# schedule(in:forMode:)

Retrieves results from a query asynchronously by scheduling the query in a run loop.

Mac CatalystmacOS 10.6+

``` source
func schedule(
    in inRunLoop: RunLoop!,
    forMode inMode: String!
)
```

## Parameters 

`inRunLoop`  

The run loop.

`inMode`  

The mode of the run loop.

## Discussion

A delegate must be set prior to calling this method; otherwise, results may be lost due to the lack of a receiver.

## See Also

### Managing Asynchronous Queries

var delegate: (any ODQueryDelegate)!

The query’s delegate.

var operationQueue: OperationQueue!

The queue on which asynchronous results are delivered to the delegate.

func remove(from: RunLoop!, forMode: String!)

Removes the query from a specified run loop.

func synchronize()

Restarts a query, disposing of any results it has obtained.

