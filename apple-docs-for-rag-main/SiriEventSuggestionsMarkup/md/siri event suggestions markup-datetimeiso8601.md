

- Siri Event Suggestions Markup
-  dateTimeISO8601 

Type

# dateTimeISO8601

A time and date in the ISO-8601 format.

Siri Event Suggestions Markup 1.0+

``` source
date-time dateTimeISO8601
```

## Possible Values 

`/^\d{4}-\d{2}-\d{2}(?:T\d{2}:\d{2}:\d{2}(?:\.\d{1,6})?(?:Z|[-\+]\d{2}:?\d{2})?)?$//`  

## Overview

Event start and end times must use the ISO-8601 format. Provide the most relevant time zone in each `dateTimeISO8601`. For example, a flight reservation from Indiana to California should provide the departure time in the local time zone at the airport in Indiana and the arrival time in California’s time zone.

## See Also

### Basic Data Types

type @context

The open standard reference for interpreting the markup contents.

type reservationId

A stable, unique identifier for the reservation.

type reservationStatus

A string indicating that the reservation has been confirmed or canceled.

type URL

The address of a webpage.

type telephone

A phone number.

