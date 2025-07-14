

- Siri Event Suggestions Markup
-  Flight 

Object

# Flight

Location and scheduling information for an airplane flight.

Siri Event Suggestions Markup 1.0+

``` source
object Flight
```

## Properties

`@type`

`string`

 (Required) 

Value: `Flight`

`arrivalAirport`

Airport

 (Required) 

The airport where the flight ends.

`arrivalGate`

`string`

The airport gate where the flight ends.

`arrivalTerminal`

`string`

The airport terminal where the flight ends.

`arrivalTime`

dateTimeISO8601

 (Required) 

The scheduled date and time, in the airport’s local time zone, that the flight ends.

`departureAirport`

Airport

 (Required) 

The airport where the flight begins.

`departureGate`

`string`

The airport gate where the flight begins.

`departureTerminal`

`string`

The airport terminal where the flight begins.

`departureTime`

dateTimeISO8601

 (Required) 

The scheduled date and time, in the airport’s local time zone, that the flight begins.

`flightNumber`

`string`

 (Required) 

The flight number, specific to an airline.

`provider`

Airline

 (Required) 

The airline providing the flight.

## See Also

### Defining a Flight Reservation

object Airline

An airline’s name and identifier.

object Airport

The name and location of an airport.

