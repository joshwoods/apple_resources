

- Core Motion
-  CMPedometerHandler 

Type Alias

# CMPedometerHandler

A block for processing pedometer-related data.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.0+macOS 10.15+watchOS 2.0+

``` source
typealias CMPedometerHandler = (CMPedometerData?, (any Error)?) -> Void
```

## Discussion

You provide a block of this type when requesting data from the `CMPedometer` object. When the data becomes available, the pedometer object delivers that data to your block for processing. If there was an error retrieving the data, the pedometer object provides an error object instead.

This block has no return value and takes the following parameters:

`pedometerData`  
A CMPedometerData object containing the available data. If there was an error retrieving the data, this parameter is `nil`.

`error`  
An NSError object if there was a problem or `nil` if the pedometer data was retrieved successfully.

## See Also

### Gathering Live Pedometer Data

func startUpdates(from: Date, withHandler: CMPedometerHandler)

Starts the delivery of recent pedestrian-related data to your app.

func stopUpdates()

Stops the delivery of recent pedestrian data updates to your app.

func startEventUpdates(handler: CMPedometerEventHandler)

Starts the delivery of pedometer events to your app.

func stopEventUpdates()

Stops the delivery of pedometer events to your app.

typealias CMPedometerEventHandler

A block for processing pedometer events.

