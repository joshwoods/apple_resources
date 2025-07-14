

- WeatherKit REST API
-  WeatherAlertSummary 

Object

# WeatherAlertSummary

Detailed information about the weather alert.

Weather API 1.0.0+

``` source
object WeatherAlertSummary
```

## Properties

`areaId`

`string`

An official designation of the affected area.

`areaName`

`string`

A human-readable name of the affected area.

`certainty`

Certainty

 (Required) 

How likely the event is to occur.

`countryCode`

`string`

 (Required) 

The ISO code of the reporting country.

`description`

`string`

 (Required) 

A human-readable description of the event.

`detailsUrl`

`string`

The URL to a page containing detailed information about the event.

`effectiveTime`

`date-time`

 (Required) 

The time the event went into effect.

`eventEndTime`

`date-time`

The time when the underlying weather event is projected to end.

`eventOnsetTime`

`date-time`

The time when the underlying weather event is projected to start.

`expireTime`

`date-time`

 (Required) 

The time when the event expires.

`id`

`uuid`

 (Required) 

A unique identifier of the event.

`issuedTime`

`date-time`

 (Required) 

The time that event was issued by the reporting agency.

`responses`

`[`ResponseType`]`

 (Required) 

An array of recommended actions from the reporting agency.

`severity`

Severity

 (Required) 

The level of danger to life and property.

`source`

`string`

 (Required) 

The name of the reporting agency.

`urgency`

Urgency

An indication of urgency of action from the reporting agency.

## Attributes 

Possible types:

## Relationships

### Inherited By

- WeatherAlert

## See Also

### Obtaining weather alerts

GET /api/v1/weatherAlert/{language}/{id}

Receive an active weather alert.

object WeatherAlert

An official message indicating severe weather from a reporting agency.

object WeatherAlertCollection

A collection of severe weather alerts for a specified location.

type ResponseType

The recommended action from a reporting agency.

type Severity

The level of danger to life and property.

type Urgency

An indication of urgency of action from the reporting agency.

