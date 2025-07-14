

- WebKit JS
-  HTMLMediaElement 

Class

# HTMLMediaElement

An abstract superclass for media classes that display audio or video in webpages. This class defines common properties and methods inherited by the HTMLAudioElement and HTMLVideoElement classes representing the HTML `audio` and `video` elements.

Safari Desktop 10.0+Safari Mobile 3.0+

``` source
interface HTMLMediaElement
```

## Overview

### Handling Events

The different types of media events that can occur are described in Table 1.

| Event | Description |
|----|----|
| `abort` | Sent when the browser stops fetching the media data before the media resource was completely downloaded. |
| `canplay` | Sent when the browser can resume playback of the media data, but estimates that if playback is started now, the media resource could not be rendered at the current playback rate up to its end without having to stop for further buffering of content. |
| `canplaythrough` | Sent when the browser estimates that if playback is started now, the media resource could be rendered at the current playback rate all the way to its end without having to stop for further buffering. |
| `durationchange` | Sent when the duration property changes. |
| `emptied` | Sent when the media element network state changes to the NETWORK_EMPTY state. |
| `ended` | Sent when playback has stopped at the end of the media resource and the ended property is set to `true`. |
| `error` | Sent when an error occurs while fetching the media data. Use the error property to get the current error. |
| `loadeddata` | Sent when the browser can render the media data at the current playback position for the first time. |
| `loadedmetadata` | Sent when the browser knows the duration and dimensions of the media resource. |
| `loadstart` | Sent when the browser begins loading the media data. |
| `pause` | Sent when playback pauses after the pause method returns. |
| `play` | Sent when playback starts after the play method returns. |
| `playing` | Sent when playback starts. |
| `progress` | Sent when the browser is fetching the media data. |
| `ratechange` | Sent when either the defaultPlaybackRate or the playbackRate property changes. |
| `seeked` | Sent when the seeking property is set to `false` |
| `seeking` | Sent when the seeking property is set to `true` and there is time to send this event. |
| `stalled` | Sent when the browser is fetching media data but it has stopped arriving. |
| `suspend` | Sent when the browser suspends loading the media data and does not have the entire media resource downloaded. |
| `timeupdate` | Sent when the currentTime property changes as part of normal playback or because of some other condition. |
| `volumechange` | Sent when either the volume property or the muted property changes. |
| `waiting` | Sent when the browser stops playback because it is waiting for the next frame. |

**Table 1** Media element events

## Topics

### Getting and Setting Properties

autoplay

A Boolean value that determines whether the media resource plays automatically when available.

controls

A Boolean value that determines whether the playback controls appear.

currentTime

The current playback position in seconds.

defaultPlaybackRate

The default rate used to play the media resource.

loop

A Boolean value that determines whether the playback should loop.

muted

A Boolean value that determines whether the audio content should be muted.

playbackRate

The speed that the media resource is playing.

preload

A DOMString value that gives a hint to the browser how much of the media should be fetched when the webpage is loaded.

src

The URI address of the media resource to play.

volume

The volume of the audio portion of the media element.

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

### Controlling Playback

canPlayType

Returns whether the media element supports the specified MIME type.

load

Starts loading the media resource.

pause

Pauses the media playback if in progress.

play

Begins playing the media resource.

### Constants

Media Ready States

Possible values for the readyState property.

Network States

Possible values for the networkState property.

### Instance Properties

audioTracks

controller

crossOrigin

defaultMuted

kind

mediaGroup

session

srcObject

textTracks

videoTracks

webkitClosedCaptionsVisible

webkitCurrentPlaybackTargetIsWireless

webkitHasClosedCaptions

webkitKeys

webkitPreservesPitch

### Instance Methods

addTextTrack

fastSeek

getStartDate

getVideoPlaybackQuality

webkitSetMediaKeys

webkitShowPlaybackTargetPicker

