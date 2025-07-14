

- Siri Event Suggestions Markup
-  Airline 

Object

# Airline

An airline’s name and identifier.

Siri Event Suggestions Markup 1.0+

``` source
object Airline
```

## Properties

`@type`

`string`

 (Required) 

Value: `Airline`

`iataCode`

`string`

 (Required) 

The three-letter identifier of the airline.

Value: `/^[A-Z]{3}$/`

`name`

`string`

 (Required) 

The name of the airline.

## See Also

### Defining a Flight Reservation

object Flight

Location and scheduling information for an airplane flight.

object Airport

The name and location of an airport.

