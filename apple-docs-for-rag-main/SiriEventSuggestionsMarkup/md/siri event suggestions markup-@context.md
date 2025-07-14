

- Siri Event Suggestions Markup
-  @context 

Type

# @context

The open standard reference for interpreting the markup contents.

Siri Event Suggestions Markup 1.0+

``` source
string @context
```

## Possible Values 

`http://schema.org`  

## Overview

For JSON-LD, the `@context` for a reservation should always be `http://schema.org`, as in this example:

```
{ "@context": "http://schema.org", "@type": "TrainReservation", "reservationId": "ASDF1234" /* more data goes here */ }}
```

For Microdata, provide the URL as part of the `itemtype`, as in this example:

```

Your reservation
ASDF1234
is confirmed!
/* more data goes here */

```

## See Also

### Basic Data Types

type dateTimeISO8601

A time and date in the ISO-8601 format.

type reservationId

A stable, unique identifier for the reservation.

type reservationStatus

A string indicating that the reservation has been confirmed or canceled.

type URL

The address of a webpage.

type telephone

A phone number.

