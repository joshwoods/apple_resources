

- Siri Event Suggestions Markup
-  EventReservation 

Object

# EventReservation

A reservation for a movie, sporting event, live show, or other scheduled event.

Siri Event Suggestions Markup 1.0+

``` source
object EventReservation
```

## Properties

`@context`

@context

 (Required) 

`@type`

`string`

 (Required) 

Value: `EventReservation`

`reservationFor`

Event

 (Required) 

General information about the event.

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

The event attendee, or a primary attendee if the event provider doesn’t require a name for each attendee.

`broker`

Organization

An intermediary booking service.

`url`

URL

A webpage the user can access to view reservation details.

## Topics

### Defining an Event Reservation

object Event

A sporting event, live show, or other scheduled event.

## See Also

### Food, Lodging, and Events

object FoodEstablishmentReservation

A restaurant reservation.

object LodgingReservation

A hotel reservation or other booking for a place to stay.

