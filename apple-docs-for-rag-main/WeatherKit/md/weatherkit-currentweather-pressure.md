

- WeatherKit
- CurrentWeather
-  pressure 

Instance Property

# pressure

The sea level air pressure in millibars.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
var pressure: Measurement
```

## Discussion

This is a reduced pressure calculated by using observed conditions to remove the effects of elevation from pressure readings.

## See Also

### Getting wind and pressure

var pressureTrend: PressureTrend

The direction of change of the sea level air pressure.

var wind: Wind

The wind speed, direction, and gust.

