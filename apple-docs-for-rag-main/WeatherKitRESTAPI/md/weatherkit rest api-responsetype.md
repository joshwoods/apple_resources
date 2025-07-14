

- WeatherKit REST API
-  ResponseType 

Type

# ResponseType

The recommended action from a reporting agency.

Weather API 1.0.0+

``` source
string ResponseType
```

## Possible Values 

`shelter`  

`evacuate`  

`prepare`  

`execute`  

`avoid`  

`monitor`  

`assess`  

`allClear`  

`none`  

## Attributes 

Possible types:

## Possible Values

shelter  
Take shelter in place.

evacuate  
Relocate.

prepare  
Make preparations.

execute  
Execute a pre-planned activity.

avoid  
Avoid the event.

monitor  
Monitor the situation.

assess  
Assess the situation.

allClear  
The event no longer poses a threat.

none  
No action recommended.

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

type Severity

The level of danger to life and property.

type Urgency

An indication of urgency of action from the reporting agency.

