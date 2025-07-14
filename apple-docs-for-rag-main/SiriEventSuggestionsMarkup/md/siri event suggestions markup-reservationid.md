

- Siri Event Suggestions Markup
-  reservationId 

Type

# reservationId

A stable, unique identifier for the reservation.

Siri Event Suggestions Markup 1.0+

``` source
string reservationId
```

## Mentioned in 

Checking Your Reservation Markup

## Discussion

Use a consistent, unique identifier for each reservation. If you also provide reservation information with doc://com.apple.documentation/documentation/sirikit/siri_event_suggestions in your app, use a single, consistent value for that doc://com.apple.documentation/documentation/sirikit/inreservation/3113835-reservationnumber and this `reservationId`.

## See Also

### Basic Data Types

type @context

The open standard reference for interpreting the markup contents.

type dateTimeISO8601

A time and date in the ISO-8601 format.

type reservationStatus

A string indicating that the reservation has been confirmed or canceled.

type URL

The address of a webpage.

type telephone

A phone number.

