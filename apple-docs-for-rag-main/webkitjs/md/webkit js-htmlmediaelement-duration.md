

- WebKit JS
- HTMLMediaElement
-  duration 

Instance Property

# duration

The length of the media resource in seconds. (read-only)

Safari Desktop 10.0+Safari Mobile 10.0+

``` source
readonly attribute unrestricted double duration;
```

## Discussion

This property is `0` if there is no media data available. This property is `NaN` if the duration is unknown. The value is positive infinity if the duration is known but is indefinite—for example, a live stream.

## See Also

### Getting State

buffered

The time ranges of the media resource that have been downloaded. (read-only)

currentSrc

The absolute URL of the media resource. (read-only)

ended

A Boolean value that indicates whether the media played to the end. (read-only)

error

The last error that occurred for this element. (read-only)

networkState

The state of downloading the media resource. (read-only)

paused

A Boolean value that indicates whether the media is paused. (read-only)

played

The ranges of the media resource that was played. (read-only)

readyState

The ready state of the media resource. (read-only)

seekable

The ranges that can be played in a nonlinear fashion. (read-only)

seeking

A Boolean value that indicates whether the element is seeking. (read-only)

startTime

The earliest possible time in seconds to start playback. (read-only)

