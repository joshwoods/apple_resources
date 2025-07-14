

- Siri Event Suggestions Markup
-  FoodEstablishmentReservation 

Object

# FoodEstablishmentReservation

A restaurant reservation.

Siri Event Suggestions Markup 1.0+

``` source
object FoodEstablishmentReservation
```

## Properties

`@context`

@context

 (Required) 

`@type`

`string`

 (Required) 

Value: `FoodEstablishmentReservation`

`partySize`

`integer`

The number of people.

`reservationFor`

FoodEstablishment

 (Required) 

The restaurant or other food establishment hosting the reservation.

`reservationId`

reservationId

 (Required) 

A unique identifier for the reservation, consistent in all markup.

`reservationStatus`

reservationStatus

 (Required) 

The reservation’s current status.

`startTime`

dateTimeISO8601

 (Required) 

The beginning date and time for the reservation.

`underName`

Person

 (Required) 

The name of the person associated with the reservation, usually someone who will be dining.

`broker`

Organization

An intermediary booking service.

`url`

URL

A webpage the user can access to view reservation details.

## Topics

### Defining a Restaurant Reservation

object FoodEstablishment

The restaurant or other food establishment that will host the reservation.

## See Also

### Food, Lodging, and Events

object EventReservation

A reservation for a movie, sporting event, live show, or other scheduled event.

object LodgingReservation

A hotel reservation or other booking for a place to stay.

