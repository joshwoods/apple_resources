

- WeatherKit REST API
- CurrentWeather
-  CurrentWeather.CurrentWeatherData 

Object

# CurrentWeather.CurrentWeatherData

The current weather object.

Weather API 1.0.0+

``` source
object CurrentWeather.CurrentWeatherData
```

## Properties

`asOf`

`date-time`

 (Required) 

The date and time.

`cloudCover`

`number`

The percentage of the sky covered with clouds during the period, from `0` to `1`.

`conditionCode`

`string`

 (Required) 

An enumeration value indicating the condition at the time.

`daylight`

`boolean`

A Boolean value indicating whether there is daylight.

`humidity`

`number`

 (Required) 

The relative humidity, from `0` to `1`.

`precipitationIntensity`

`number`

 (Required) 

The precipitation intensity, in millimeters per hour.

`pressure`

`number`

 (Required) 

The sea level air pressure, in millibars.

`pressureTrend`

PressureTrend

 (Required) 

The direction of change of the sea-level air pressure.

`temperature`

`number`

 (Required) 

The current temperature, in degrees Celsius.

`temperatureApparent`

`number`

 (Required) 

The feels-like temperature when factoring wind and humidity, in degrees Celsius.

`temperatureDewPoint`

`number`

 (Required) 

The temperature at which relative humidity is 100%, in Celsius.

`uvIndex`

`integer`

 (Required) 

The level of ultraviolet radiation.

`visibility`

`number`

 (Required) 

The distance at which terrain is visible, in meters.

`windDirection`

`integer`

The direction of the wind, in degrees.

`windGust`

`number`

The maximum wind gust speed, in kilometers per hour.

`windSpeed`

`number`

 (Required) 

The wind speed, in kilometers per hour.

## Attributes 

Possible types:

## Relationships

### Inherited By

- CurrentWeather

