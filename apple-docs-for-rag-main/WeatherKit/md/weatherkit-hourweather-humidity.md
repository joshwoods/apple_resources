

- WeatherKit
- HourWeather
-  humidity 

Instance Property

# humidity

The humidity for the hour.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
var humidity: Double
```

## Discussion

Relative humidity measures the amount of water vapor in the air compared to the maximum amount that the air could normally hold at the current temperature. The value is from `0` (no humidity) to `1` (100% humidity).

## See Also

### Getting temperature and humidity

var apparentTemperature: Measurement&lt;UnitTemperature>

The apparent, or “feels like” temperature during the hour.

var temperature: Measurement&lt;UnitTemperature>

The temperature during the hour.

var dewPoint: Measurement&lt;UnitTemperature>

The amount of moisture in the air.

