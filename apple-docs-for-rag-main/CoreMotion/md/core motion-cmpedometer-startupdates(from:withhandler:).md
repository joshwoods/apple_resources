

- Core Motion
- CMPedometer
-  startUpdates(from:withHandler:) 

Instance Method

# startUpdates(from:withHandler:)

Starts the delivery of recent pedestrian-related data to your app.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.15+watchOS 2.0+

``` source
func startUpdates(
    from start: Date,
    withHandler handler: @escaping CMPedometerHandler
)
```

## Parameters 

`start`  

The date from which to start reporting data. You can specify a date in the past to retrieve the data from that time until now. This parameter must not be `nil`.

`handler`  

The block to execute when data is available. This block is called repeatedly on a background thread as new data arrives. This parameter must not be `nil`. For information about this block, see CMPedometerHandler.

## Discussion

Upon calling this method, the pedometer object starts calling your handler block regularly with data. The data passed to your `handler` block represents the cumulative data starting at the specified `start` date and ending at the current time. (You can get the start and end dates from the CMPedometerData object passed to your handler.) This method initiates the event delivery process asynchronously and executes your block on a serial dispatch queue, which ensures that only one copy of the block runs at any given time.

When the app is suspended, the delivery of updates stops temporarily. Upon returning to foreground or background execution, the pedometer object begins updates again.

To stop the delivery of events, call the stopUpdates() method.

It is safe to start the delivery of events using this method and then perform additional queries using the queryPedometerData(from:to:withHandler:) method.

## See Also

### Gathering Live Pedometer Data

func stopUpdates()

Stops the delivery of recent pedestrian data updates to your app.

func startEventUpdates(handler: CMPedometerEventHandler)

Starts the delivery of pedometer events to your app.

func stopEventUpdates()

Stops the delivery of pedometer events to your app.

typealias CMPedometerHandler

A block for processing pedometer-related data.

typealias CMPedometerEventHandler

A block for processing pedometer events.

