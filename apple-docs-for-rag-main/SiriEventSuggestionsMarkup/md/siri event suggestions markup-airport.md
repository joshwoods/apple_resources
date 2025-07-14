

- Siri Event Suggestions Markup
-  Airport 

Object

# Airport

The name and location of an airport.

Siri Event Suggestions Markup 1.0+

``` source
object Airport
```

## Properties

`@type`

`string`

 (Required) 

Value: `Airport`

`iataCode`

`string`

 (Required) 

The airport’s official three-letter identifier.

Value: `/^[A-Z]{3}$/`

`name`

`string`

The name of the airport.

`address`

PostalAddress

The location of the airport.

## See Also

### Defining a Flight Reservation

object Flight

Location and scheduling information for an airplane flight.

object Airline

An airline’s name and identifier.

