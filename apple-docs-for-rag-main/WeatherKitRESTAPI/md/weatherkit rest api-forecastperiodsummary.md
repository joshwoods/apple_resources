

- WeatherKit REST API
-  ForecastPeriodSummary 

Object

# ForecastPeriodSummary

The summary for a specified period in the minute forecast.

Weather API 1.0.0+

``` source
object ForecastPeriodSummary
```

## Properties

`condition`

PrecipitationType

 (Required) 

The type of precipitation forecasted.

`endTime`

`date-time`

The end time of the forecast.

`precipitationChance`

`number`

 (Required) 

The probability of precipitation during this period.

`precipitationIntensity`

`number`

 (Required) 

The precipitation intensity in millimeters per hour.

`startTime`

`date-time`

 (Required) 

The start time of the forecast.

## Attributes 

Possible types:

## See Also

### Obtaining minute-to-minute forecast weather

object ForecastMinute

The precipitation forecast for a specified minute.

