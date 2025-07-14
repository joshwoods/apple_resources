

- WeatherKit
- Wind
-  compassDirection 

Instance Property

# compassDirection

The general indicator of wind direction.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
var compassDirection: Wind.CompassDirection
```

## Discussion

This structure refers to the direction the wind is coming from; for instance, a north wind blows from north to south.

## See Also

### Getting the properties

enum CompassDirection

A compass composed of cardinal and intercardinal directions.

var direction: Measurement&lt;UnitAngle>

The direction the wind is coming from in degrees.

var gust: Measurement&lt;UnitSpeed>?

A sudden increase in wind speed due to friction, wind shear, or by heating.

var speed: Measurement&lt;UnitSpeed>

Sustained wind speed.

