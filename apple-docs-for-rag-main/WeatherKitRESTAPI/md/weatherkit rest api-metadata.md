

- WeatherKit REST API
-  Metadata 

Object

# Metadata

Descriptive information about the weather data.

Weather API 1.0.0+

``` source
object Metadata
```

## Properties

`attributionURL`

`string`

The URL of the legal attribution for the data source.

`expireTime`

`date-time`

 (Required) 

The time when the weather data is no longer valid.

`language`

`string`

The ISO language code for localizable fields.

`latitude`

`number`

 (Required) 

The latitude of the relevant location.

`longitude`

`number`

 (Required) 

The longitude of the relevant location.

`providerLogo`

`string`

The URL of a logo for the data provider.

`providerName`

`string`

The name of the data provider.

`readTime`

`date-time`

 (Required) 

The time the weather data was procured.

`reportedTime`

`date-time`

The time the provider reported the weather data.

`temporarilyUnavailable`

`boolean`

The weather data is temporarily unavailable from the provider.

`units`

UnitsSystem

The system of units that the weather data is reported in. This is set to metric.

`version`

`integer`

 (Required) 

The data format version.

## Attributes 

Possible types:

## See Also

### Obtaining current weather information

object CurrentWeather

The current weather conditions for the specified location.

object ProductData

A base type for all weather data.

