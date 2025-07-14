

- WeatherKit
- Wind
-  direction 

Instance Property

# direction

The direction the wind is coming from in degrees.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
var direction: Measurement
```

## Discussion

True north is at `0` degrees and progresses clockwise from north.

## See Also

### Getting the properties

enum CompassDirection

A compass composed of cardinal and intercardinal directions.

var compassDirection: Wind.CompassDirection

The general indicator of wind direction.

var gust: Measurement&lt;UnitSpeed>?

A sudden increase in wind speed due to friction, wind shear, or by heating.

var speed: Measurement&lt;UnitSpeed>

Sustained wind speed.

