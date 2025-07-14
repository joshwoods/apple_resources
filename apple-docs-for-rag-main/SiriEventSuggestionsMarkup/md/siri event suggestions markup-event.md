

- Siri Event Suggestions Markup
-  Event 

Object

# Event

A sporting event, live show, or other scheduled event.

Siri Event Suggestions Markup 1.0+

``` source
object Event
```

## Properties

`@type`

`string`

 (Required) 

Possible Values: `Event, ScreeningEvent`

`location`

Place

 (Required) 

The venue hosting the event.

`name`

`string`

 (Required) 

The name of the event.

`startDate`

dateTimeISO8601

 (Required) 

The time and date the event starts.

`endDate`

dateTimeISO8601

The time and date the event ends.

