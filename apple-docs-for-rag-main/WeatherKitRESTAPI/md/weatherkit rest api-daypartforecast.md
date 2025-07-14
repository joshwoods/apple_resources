

- WeatherKit REST API
-  DayPartForecast 

Object

# DayPartForecast

A summary forecast for a daytime or overnight period.

Weather API 1.0.0+

``` source
object DayPartForecast
```

## Properties

`cloudCover`

`number`

 (Required) 

The percentage of the sky covered with clouds during the period, from `0` to `1`.

`conditionCode`

`string`

 (Required) 

An enumeration value indicating the condition at the time.

`forecastEnd`

`date-time`

 (Required) 

The ending date and time of the forecast.

`forecastStart`

`date-time`

 (Required) 

The starting date and time of the forecast.

`humidity`

`number`

 (Required) 

The relative humidity during the period, from `0` to `1`.

`precipitationAmount`

`number`

 (Required) 

The amount of precipitation forecasted to occur during the period, in millimeters.

`precipitationChance`

`number`

 (Required) 

The chance of precipitation forecasted to occur during the period.

`precipitationType`

PrecipitationType

 (Required) 

The type of precipitation forecasted to occur during the period.

`snowfallAmount`

`number`

 (Required) 

The depth of snow as ice crystals forecasted to occur during the period, in millimeters.

`windDirection`

`integer`

The direction the wind is forecasted to come from during the period, in degrees.

`windSpeed`

`number`

 (Required) 

The average speed the wind is forecasted to be during the period, in kilometers per hour.

## Attributes 

Possible types:

## See Also

### Obtaining daily weather information

object DayWeatherConditions

The historical or forecasted weather conditions for a specified day.

object DailyForecast

A collection of day forecasts for a specified range of days.

