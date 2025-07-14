

- Siri Event Suggestions Markup
-  BoatReservation 

Object

# BoatReservation

A reservation for boat travel.

Siri Event Suggestions Markup 1.0+

``` source
object BoatReservation
```

## Properties

`@context`

@context

 (Required) 

`@type`

`string`

 (Required) 

Value: `BoatReservation`

`reservationFor`

BoatTrip

 (Required) 

Details about the boat trip.

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

Details about the passenger’s ticket.

`underName`

Person

 (Required) 

The passenger, or the primary passenger of a multiperson reservation if the provider doesn’t require a name for each passenger.

`broker`

Organization

An intermediary booking service.

`url`

URL

A webpage the user can access to view reservation details.

## Topics

### Defining a Boat Reservation

object BoatTrip

Location and scheduling information for a boat trip.

object BoatTerminal

The name and location of a boat terminal.

## See Also

### Transportation

object FlightReservation

An airplane flight reservation.

object TrainReservation

A reservation for train travel.

object BusReservation

A reservation for bus travel.

object RentalCarReservation

A reservation to rent a car.

