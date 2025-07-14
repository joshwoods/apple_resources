

- WeatherKit REST API
-  Urgency 

Type

# Urgency

An indication of urgency of action from the reporting agency.

Weather API 1.0.0+

``` source
string Urgency
```

## Possible Values 

`immediate`  

`expected`  

`future`  

`past`  

`unknown`  

## Attributes 

Possible types:

## Possible Values

immediate  
Take responsive action immediately.

expected  
Take responsive action in the next hour.

future  
Take responsive action in the near future.

past  
Responsive action is no longer required.

unknown  
The urgency is unknown.

## See Also

### Obtaining weather alerts

GET /api/v1/weatherAlert/{language}/{id}

Receive an active weather alert.

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

