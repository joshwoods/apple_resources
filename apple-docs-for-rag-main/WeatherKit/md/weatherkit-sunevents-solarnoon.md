

- WeatherKit
- SunEvents
-  solarNoon 

Instance Property

# solarNoon

Represents solar noon, the time when the sun reaches its highest point in the sky.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
var solarNoon: Date?
```

## Discussion

It may or may not be above the horizon at this time due to variations of solar events at extreme latitudes. If the highest point isn’t above the horizon, this property is `nil`.

## See Also

### Getting the sun events

var astronomicalDawn: Date?

The time of astronomical sunrise when the sun’s center is 18° below the horizon.

var astronomicalDusk: Date?

The time of astronomical sunset, when the sun’s center is 18° below the horizon.

var civilDawn: Date?

The time of civil sunrise when the sun’s center is 6° below the horizon.

var civilDusk: Date?

The time of civil sunset, when the sun’s center is 6° below the horizon.

var nauticalDawn: Date?

The time of nautical sunrise when the sun’s center is 12° below the horizon.

var nauticalDusk: Date?

The time of nautical sunset, when the sun’s center is 12° below the horizon.

var solarMidnight: Date?

Represents solar midnight, the time when the sun reaches its lowest point in the sky.

var sunrise: Date?

The sunrise time immediately before the solar transit closest to calendar noon.

var sunset: Date?

The sunset time immediately after the solar transit closest to calendar noon.

