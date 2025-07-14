

- Siri Event Suggestions Markup
-  LodgingReservation 

Object

# LodgingReservation

A hotel reservation or other booking for a place to stay.

Siri Event Suggestions Markup 1.0+

``` source
object LodgingReservation
```

## Properties

`@context`

@context

 (Required) 

`@type`

`string`

 (Required) 

Value: `LodgingReservation`

`checkinTime`

dateTimeISO8601

 (Required) 

The earliest the guest may check in.

`checkoutTime`

dateTimeISO8601

 (Required) 

The latest the guest may check out.

`reservationFor`

LodgingBusiness

 (Required) 

The location of the lodging, such as a hotel or inn.

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

The lodging guest, or a primary guest if the event provider doesn’t require a name for each guest.

`broker`

Organization

An intermediary booking service.

`url`

URL

A webpage the user can access to view reservation details.

## Topics

### Defining a Lodging Reservation

object LodgingBusiness

A hotel, inn, or other lodging location.

## See Also

### Food, Lodging, and Events

object EventReservation

A reservation for a movie, sporting event, live show, or other scheduled event.

object FoodEstablishmentReservation

A restaurant reservation.

