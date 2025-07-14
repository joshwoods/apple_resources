

- RealityKit
- ActionAnimation
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

