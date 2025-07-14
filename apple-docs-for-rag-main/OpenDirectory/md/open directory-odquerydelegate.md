

- Open Directory
-  ODQueryDelegate 

Protocol

# ODQueryDelegate

The `ODQueryDelegate` protocol defines methods for receiving results returned from an Open Directory query.

Mac CatalystmacOS

``` source
protocol ODQueryDelegate : NSObjectProtocol
```

## Topics

### Receiving results from a scheduled query

func query(ODQuery!, foundResults: [Any]!, error: (any Error)!)

The delegate method called as results are returned from a query scheduled in a run loop.

**Required**

## Relationships

### Inherits From

- NSObjectProtocol

