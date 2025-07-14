

- WeatherKit
- SunEvents
-  astronomicalDawn 

Instance Property

# astronomicalDawn

The time of astronomical sunrise when the sun’s center is 18° below the horizon.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
var astronomicalDawn: Date?
```

## Discussion

A small portion of the sun’s rays begin to illuminate the sky and stars begin to disappear. This property is optional because it’s possible for the sun to not rise on a given day, at extreme latitudes.

## See Also

### Getting the sun events

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

var solarNoon: Date?

Represents solar noon, the time when the sun reaches its highest point in the sky.

var sunrise: Date?

The sunrise time immediately before the solar transit closest to calendar noon.

var sunset: Date?

The sunset time immediately after the solar transit closest to calendar noon.

