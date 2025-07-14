

- WeatherKit REST API
-  WeatherAlert 

Object

# WeatherAlert

An official message indicating severe weather from a reporting agency.

Weather API 1.0.0+

``` source
object WeatherAlert
```

## Attributes 

Possible types:

## Topics

### Getting the weather alert

object WeatherAlert.WeatherAlertData

The weather alert information.

## Relationships

### Inherits From

- WeatherAlert.WeatherAlertData
- WeatherAlertSummary

## See Also

### Obtaining weather alerts

GET /api/v1/weatherAlert/{language}/{id}

Receive an active weather alert.

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

