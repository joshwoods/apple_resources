

- Siri Event Suggestions Markup
-  BoatTrip 

Object

# BoatTrip

Location and scheduling information for a boat trip.

Siri Event Suggestions Markup 1.0+

``` source
object BoatTrip
```

## Properties

`@type`

`string`

 (Required) 

Value: `BoatTrip`

`arrivalBoatTerminal`

BoatTerminal

 (Required) 

The terminal where the boat reservation ends.

`arrivalTime`

dateTimeISO8601

 (Required) 

The scheduled time the boat arrives.

`departureBoatTerminal`

BoatTerminal

 (Required) 

The terminal where the boat reservation begins.

`departureTime`

dateTimeISO8601

 (Required) 

The scheduled time the boat departs.

`identifier`

`string`

 (Required) 

The boat’s number or other identifier.

`name`

`string`

 (Required) 

The boat or boat route’s name.

`provider`

Organization

The organization providing the boat trip.

## See Also

### Defining a Boat Reservation

object BoatTerminal

The name and location of a boat terminal.

