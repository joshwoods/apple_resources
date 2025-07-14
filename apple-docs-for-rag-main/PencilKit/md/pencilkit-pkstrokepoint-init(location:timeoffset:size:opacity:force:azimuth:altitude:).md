

- PencilKit
- PKStrokePoint
-  init(location:timeOffset:size:opacity:force:azimuth:altitude:) 

Initializer

# init(location:timeOffset:size:opacity:force:azimuth:altitude:)

Creates a new point with the provided properties.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+visionOS 1.0+

``` source
init(
    location: CGPoint,
    timeOffset: TimeInterval,
    size: CGSize,
    opacity: CGFloat,
    force: CGFloat,
    azimuth: CGFloat,
    altitude: CGFloat
)
```

## Parameters 

`location`  

The location of this point.

`timeOffset`  

The time offset since the start of this stoke path in seconds.

`size`  

The size of this point.

`opacity`  

The opacity of this point, ranging from `0` to `2`.

`force`  

The amount of force used to create this point.

`azimuth`  

The azimuth of this point in radians.

`altitude`  

The altitude of this point in radians.

## See Also

### Creating a stroke point object

init(location: CGPoint, timeOffset: TimeInterval, size: CGSize, opacity: CGFloat, force: CGFloat, azimuth: CGFloat, altitude: CGFloat, secondaryScale: CGFloat)

