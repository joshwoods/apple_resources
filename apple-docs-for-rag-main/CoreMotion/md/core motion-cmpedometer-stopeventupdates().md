

- Core Motion
- CMPedometer
-  stopEventUpdates() 

Instance Method

# stopEventUpdates()

Stops the delivery of pedometer events to your app.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+watchOS 3.0+

``` source
func stopEventUpdates()
```

## See Also

### Gathering Live Pedometer Data

func startUpdates(from: Date, withHandler: CMPedometerHandler)

Starts the delivery of recent pedestrian-related data to your app.

func stopUpdates()

Stops the delivery of recent pedestrian data updates to your app.

func startEventUpdates(handler: CMPedometerEventHandler)

Starts the delivery of pedometer events to your app.

typealias CMPedometerHandler

A block for processing pedometer-related data.

typealias CMPedometerEventHandler

A block for processing pedometer events.

