

- Siri Event Suggestions Markup
-  TrainReservation 

Object

# TrainReservation

A reservation for train travel.

Siri Event Suggestions Markup 1.0+

``` source
object TrainReservation
```

## Properties

`@context`

@context

 (Required) 

`@type`

`string`

 (Required) 

Value: `TrainReservation`

`reservationFor`

TrainTrip

 (Required) 

Details about the train trip.

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

### Defining a Train Reservation

object TrainTrip

Location and scheduling information for a train trip.

object TrainStation

The name and location of a train station.

## See Also

### Transportation

object FlightReservation

An airplane flight reservation.

object BusReservation

A reservation for bus travel.

object BoatReservation

A reservation for boat travel.

object RentalCarReservation

A reservation to rent a car.

