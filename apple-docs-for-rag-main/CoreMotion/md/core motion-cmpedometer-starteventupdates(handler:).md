

- Core Motion
- CMPedometer
-  startEventUpdates(handler:) 

Instance Method

# startEventUpdates(handler:)

Starts the delivery of pedometer events to your app.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+watchOS 3.0+

``` source
func startEventUpdates(handler: @escaping CMPedometerEventHandler)
```

## Parameters 

`handler`  

The block to execute when a pedometer event is available. This parameter must not be `nil`.

## Discussion

Pedometer events report changes in the user’s pedestrian activity.

## See Also

### Gathering Live Pedometer Data

func startUpdates(from: Date, withHandler: CMPedometerHandler)

Starts the delivery of recent pedestrian-related data to your app.

func stopUpdates()

Stops the delivery of recent pedestrian data updates to your app.

func stopEventUpdates()

Stops the delivery of pedometer events to your app.

typealias CMPedometerHandler

A block for processing pedometer-related data.

typealias CMPedometerEventHandler

A block for processing pedometer events.

