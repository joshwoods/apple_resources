

- WebKit JS
- HTMLMediaElement
-  networkState 

Instance Property

# networkState

The state of downloading the media resource. (read-only)

Safari Desktop 3.1+Safari Mobile 3.0+

``` source
readonly attribute unsigned short networkState;
```

## Discussion

Possible values are described in Network States.

## See Also

### Getting State

buffered

The time ranges of the media resource that have been downloaded. (read-only)

currentSrc

The absolute URL of the media resource. (read-only)

duration

The length of the media resource in seconds. (read-only)

ended

A Boolean value that indicates whether the media played to the end. (read-only)

error

The last error that occurred for this element. (read-only)

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

