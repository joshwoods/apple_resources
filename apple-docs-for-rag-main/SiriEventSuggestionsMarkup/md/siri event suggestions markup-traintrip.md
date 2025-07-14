

- Siri Event Suggestions Markup
-  TrainTrip 

Object

# TrainTrip

Location and scheduling information for a train trip.

Siri Event Suggestions Markup 1.0+

``` source
object TrainTrip
```

## Properties

`@type`

`string`

 (Required) 

Value: `TrainTrip`

`arrivalStation`

TrainStation

 (Required) 

The station where the train reservation ends.

`arrivalTime`

dateTimeISO8601

 (Required) 

The scheduled time the train arrives.

`departureStation`

TrainStation

 (Required) 

The station where the train reservation starts.

`departureTime`

dateTimeISO8601

 (Required) 

The scheduled time the train departs.

`trainName`

`string`

 (Required) 

The name of the train.

`trainNumber`

`string`

 (Required) 

The train’s route number or other identifier.

`provider`

Organization

The railway providing the train trip.

`arrivalPlatform`

`string`

`departurePlatform`

`string`

## See Also

### Defining a Train Reservation

object TrainStation

The name and location of a train station.

