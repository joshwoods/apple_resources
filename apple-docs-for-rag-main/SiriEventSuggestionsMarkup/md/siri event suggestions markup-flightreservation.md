

- Siri Event Suggestions Markup
-  FlightReservation 

Object

# FlightReservation

An airplane flight reservation.

Siri Event Suggestions Markup 1.0+

``` source
object FlightReservation
```

## Properties

`@context`

@context

 (Required) 

`@type`

`string`

 (Required) 

Value: `FlightReservation`

`reservationFor`

Flight

 (Required) 

Details about the flight.

`reservationId`

reservationId

 (Required) 

A unique identifier for the reservation, consistent in all markup.

`reservationStatus`

reservationStatus

 (Required) 

The reservation’s current status.

`reservedTicket`

Ticket

Details about the attendee’s ticketed seat.

`underName`

Person

 (Required) 

The passenger, or a primary passenger if the event provider doesn’t require a name for each passenger.

`broker`

Organization

An intermediary booking service.

`url`

URL

A webpage the user can access to view reservation details.

## Topics

### Defining a Flight Reservation

object Flight

Location and scheduling information for an airplane flight.

object Airline

An airline’s name and identifier.

object Airport

The name and location of an airport.

## See Also

### Transportation

object TrainReservation

A reservation for train travel.

object BusReservation

A reservation for bus travel.

object BoatReservation

A reservation for boat travel.

object RentalCarReservation

A reservation to rent a car.

