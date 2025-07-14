

- WeatherKit REST API
-  HourWeatherConditions 

Object

# HourWeatherConditions

The historical or forecasted weather conditions for a specified hour.

Weather API 1.0.0+

``` source
object HourWeatherConditions
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

`daylight`

`boolean`

Indicates whether the hour starts during the day or night.

`forecastStart`

`date-time`

 (Required) 

The starting date and time of the forecast.

`humidity`

`number`

 (Required) 

The relative humidity at the start of the hour, from `0` to `1`.

`precipitationChance`

`number`

 (Required) 

The chance of precipitation forecasted to occur during the hour, from `0` to `1`.

`precipitationType`

PrecipitationType

 (Required) 

The type of precipitation forecasted to occur during the period.

`pressure`

`number`

 (Required) 

The sea-level air pressure, in millibars.

`pressureTrend`

PressureTrend

The direction of change of the sea-level air pressure.

`snowfallIntensity`

`number`

The rate at which snow crystals are falling, in millimeters per hour.

`temperature`

`number`

 (Required) 

The temperature at the start of the hour, in degrees Celsius.

`temperatureApparent`

`number`

 (Required) 

The feels-like temperature when considering wind and humidity, at the start of the hour, in degrees Celsius.

`temperatureDewPoint`

`number`

The temperature at which relative humidity is 100% at the top of the hour, in degrees Celsius.

`uvIndex`

`integer`

 (Required) 

The level of ultraviolet radiation at the start of the hour.

`visibility`

`number`

 (Required) 

The distance at which terrain is visible at the start of the hour, in meters.

`windDirection`

`integer`

The direction of the wind at the start of the hour, in degrees.

`windGust`

`number`

The maximum wind gust speed during the hour, in kilometers per hour.

`windSpeed`

`number`

 (Required) 

The wind speed at the start of the hour, in kilometers per hour.

`precipitationAmount`

`number`

The amount of precipitation forecasted to occur during period, in millimeters.

## Attributes 

Possible types:

## See Also

### Obtaining hourly weather information

object HourlyForecast

A collection of hour forecasts for a specified range of hours.

object NextHourForecast

A minute-by-minute forecast for the next hour.

