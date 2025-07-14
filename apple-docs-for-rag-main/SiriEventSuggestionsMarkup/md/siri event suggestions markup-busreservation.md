

- Siri Event Suggestions Markup
-  BusReservation 

Object

# BusReservation

A reservation for bus travel.

Siri Event Suggestions Markup 1.0+

``` source
object BusReservation
```

## Properties

`@context`

@context

 (Required) 

`@type`

`string`

 (Required) 

Value: `BusReservation`

`reservationFor`

BusTrip

 (Required) 

Details about the bus trip.

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

### Defining a Bus Reservation

object BusTrip

Location and scheduling information for a bus trip.

object BusStation

The name and location of a bus station.

## See Also

### Transportation

object FlightReservation

An airplane flight reservation.

object TrainReservation

A reservation for train travel.

object BoatReservation

A reservation for boat travel.

object RentalCarReservation

A reservation to rent a car.

