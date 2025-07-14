

- WeatherKit REST API
-  GET /api/v1/weatherAlert/{language}/{id} 

Web Service Endpoint

# GET /api/v1/weatherAlert/{language}/{id}

Receive an active weather alert.

Weather API 1.0.0+

## URL

``` source
GET https://weatherkit.apple.com/api/v1/weatherAlert/{language}/{id}
```

## Path Parameters

`id`

`uuid`

 (Required) 

The unique identifier for the weather alert.

`language`

`string`

 (Required) 

The language tag to use for localizing responses.

## Response Codes

` 200 ``OK`

WeatherAlert

`OK`

The request is successful. The weather alert is in the response.

Content-Type: application/json

` 400 ``Bad Request`

`Bad Request`

The server is unable to process the request due to an invalid parameter value.

` 401 ``Unauthorized`

`Unauthorized`

The request isn’t authorized or doesn’t include the correct authentication information.

` 404 ``Not Found`

`Not Found`

There’s no active alert for the specified unique identifier.

## See Also

### Obtaining weather alerts

object WeatherAlert

An official message indicating severe weather from a reporting agency.

object WeatherAlertCollection

A collection of severe weather alerts for a specified location.

object WeatherAlertSummary

Detailed information about the weather alert.

type ResponseType

The recommended action from a reporting agency.

type Severity

The level of danger to life and property.

type Urgency

An indication of urgency of action from the reporting agency.

