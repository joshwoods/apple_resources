

- Siri Event Suggestions Markup
-  BusTrip 

Object

# BusTrip

Location and scheduling information for a bus trip.

Siri Event Suggestions Markup 1.0+

``` source
object BusTrip
```

## Properties

`@type`

`string`

 (Required) 

Value: `BusTrip`

`arrivalBusStop`

BusStation

 (Required) 

The station where the bus reservation ends.

`arrivalTime`

dateTimeISO8601

 (Required) 

The scheduled time the bus arrives.

`busName`

`string`

 (Required) 

The name of the bus.

`busNumber`

`string`

 (Required) 

The bus’s route number or other identifier.

`departureBusStop`

BusStation

 (Required) 

The station where the bus reservation starts.

`departureTime`

dateTimeISO8601

 (Required) 

The scheduled time the bus departs.

`provider`

Organization

The bus company.

## See Also

### Defining a Bus Reservation

object BusStation

The name and location of a bus station.

