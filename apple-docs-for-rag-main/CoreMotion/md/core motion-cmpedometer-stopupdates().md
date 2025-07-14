

- Core Motion
- CMPedometer
-  stopUpdates() 

Instance Method

# stopUpdates()

Stops the delivery of recent pedestrian data updates to your app.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.15+watchOS 2.0+

``` source
func stopUpdates()
```

## Discussion

Use this method to stop the delivery of continuous updates that were initiated by a call to the startUpdates(from:withHandler:) method.

## See Also

### Gathering Live Pedometer Data

func startUpdates(from: Date, withHandler: CMPedometerHandler)

Starts the delivery of recent pedestrian-related data to your app.

func startEventUpdates(handler: CMPedometerEventHandler)

Starts the delivery of pedometer events to your app.

func stopEventUpdates()

Stops the delivery of pedometer events to your app.

typealias CMPedometerHandler

A block for processing pedometer-related data.

typealias CMPedometerEventHandler

A block for processing pedometer events.

