

- WeatherKit REST API
-  Severity 

Type

# Severity

The level of danger to life and property.

Weather API 1.0.0+

``` source
string Severity
```

## Possible Values 

`extreme`  

`severe`  

`moderate`  

`minor`  

`unknown`  

## Attributes 

Possible types:

## Possible Values

extreme  
Extraordinary threat.

severe  
Significant threat.

moderate  
Possible threat.

minor  
Minimal or no known threat.

unknown  
Unknown threat.

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

type Urgency

An indication of urgency of action from the reporting agency.

