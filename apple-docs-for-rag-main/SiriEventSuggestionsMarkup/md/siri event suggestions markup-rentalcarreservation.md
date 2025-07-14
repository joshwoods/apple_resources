

- Siri Event Suggestions Markup
-  RentalCarReservation 

Object

# RentalCarReservation

A reservation to rent a car.

Siri Event Suggestions Markup 1.0+

``` source
object RentalCarReservation
```

## Properties

`@context`

@context

 (Required) 

`@type`

`string`

 (Required) 

Value: `RentalCarReservation`

`dropoffLocation`

Place

 (Required) 

The place where the renter returns the car.

`dropoffTime`

dateTimeISO8601

 (Required) 

The latest time the renter may return the car.

`pickupLocation`

Place

 (Required) 

The place where the renter picks up the car.

`pickupTime`

dateTimeISO8601

 (Required) 

The earliest time the driver may pick up the car.

`reservationFor`

Car

 (Required) 

The type of vehicle to be rented.

`reservationId`

reservationId

 (Required) 

A unique identifier for the reservation, consistent in all markup.

`reservationStatus`

reservationStatus

 (Required) 

The reservation’s current status.

`underName`

Person

 (Required) 

The person renting the car.

`provider`

Organization

The rental car agency.

`broker`

Organization

An intermediary booking service.

`url`

URL

A webpage the user can access to view reservation details.

## Topics

### Defining a Rental Car Reservation

object Car

A description of a rental vehicle.

object Brand

A car brand.

## See Also

### Transportation

object FlightReservation

An airplane flight reservation.

object TrainReservation

A reservation for train travel.

object BusReservation

A reservation for bus travel.

object BoatReservation

A reservation for boat travel.

