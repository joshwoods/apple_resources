

- WeatherKit
-  DayPartForecast 

Structure

# DayPartForecast

A structure that represents the weather forecast for part of the day.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
struct DayPartForecast
```

## Topics

### Instance Properties

var cloudCover: Double

The percentage of the sky covered with clouds.

var cloudCoverByAltitude: CloudCoverByAltitude

The fraction of sky obscured by low altitude, medium altitude, and high altitude clouds.

var condition: WeatherCondition

A description of the weather condition

var highTemperature: Measurement&lt;UnitTemperature>

The high temperature for the day part.

var highWindSpeed: Measurement&lt;UnitSpeed>

The maximum sustained wind speed for the day part.

var lowTemperature: Measurement&lt;UnitTemperature>

The overnight low temperature for the day part.

var maximumHumidity: Double

The maximum humidity for the day part. Relative humidity measures the amount of water vapor in the air, compared to the maximum amount that the air can hold at the current temperature.

var maximumVisibility: Measurement&lt;UnitLength>

The maximum visibility for the day part.

var minimumHumidity: Double

The minimum humidity for the day part. Relative humidity measures the amount of water vapor in the air, compared to the maximum amount that the air can hold at the current temperature.

var minimumVisibility: Measurement&lt;UnitLength>

The minimum visibility for the day part.

var precipitation: Precipitation

The description of precipitation for the day part.

var precipitationAmountByType: PrecipitationAmountByType

A breakdown of all precipitation forecasted for the day.

var precipitationChance: Double

The probability of precipitation for the day part.

var wind: Wind

Wind data describing the wind speed, direction, and gust.

