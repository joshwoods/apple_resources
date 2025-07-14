

- RealityKit
- AnimationDefinition
-  trimmed(start:end:duration:) 

Instance Method

# trimmed(start:end:duration:)

Edits the animation duration according to the specified time.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS

``` source
func trimmed(
    start: TimeInterval? = nil,
    end: TimeInterval? = nil,
    duration: TimeInterval? = nil
) -> Self
```

## Parameters 

`start`  

The time within the underlying duration to begin playback.

`end`  

The time within the underlying duration to end playback.

`duration`  

The amount of time that overrides the underlying duration.

## Return Value

A version of the animation shortened or lengthened according to the specified times.

## Discussion

If an argument property lies outside the underlying duration, the animation plays back according to the characteristics of its repeatMode.

## See Also

### Timing the animation

var speed: Float

A factor that increases or decreases the animation’s rate of playback.

**Required**

var delay: TimeInterval

An amount of time that elapses before the animation plays.

**Required**

var duration: TimeInterval

The total playback time of the animation.

**Required**

var offset: TimeInterval

The time, in seconds, at which the animation begins within the duration.

**Required**

var trimDuration: TimeInterval?

An optional duration that overrides the source animation’s duration.

**Required**

var trimStart: TimeInterval?

The time, in seconds, at which the animation plays.

**Required**

var trimEnd: TimeInterval?

The time, in seconds, at which the source animation stops.

**Required**

