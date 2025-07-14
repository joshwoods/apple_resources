

- LivePhotosKit JS
-  LivePhotosKit.Player 

Class

# LivePhotosKit.Player

A player for Live Photos.

LivePhotosKit JS 1.0+

``` source
interface LivePhotosKit.Player
```

## Overview

This class provides a default native control allowing users to play Live Photos.

On a desktop browser, when the user moves the pointer over the native control badge, the video starts playing until the user moves the pointer away from the badge or the video ends. If the user moves the pointer before the video ends, the video stops.

On a mobile device, when the user presses the Live Photo, the video starts playing until the user stops pressing or the video ends.

### Player Events

During the life cycle of a player, several events are generated. Adding an event listener to the player allows reaction to these events.

#### videoload

The player emits a `videoload` event after the video component of the Live Photo has finished loading but before the minimum number of frames necessary for smooth playback are decoded. Under normal circumstances, the `canplay` event is emitted after the `videoload` event. The event handler is then passed an `Event` object. The `Player` reference is accessible from the event’s target member.

```
player.addEventListener('videoload', (ev) => {
    // Handle event.
})
```

#### photoload

The player emits a `photoload` event when the photo component of the Live Photo has finished loading. The event handler is then passed an `Event` object. The Player reference is accessible from the event’s target member.

```
player.addEventListener('photoload', (ev) => {
    // Handle event.
})
```

#### canplay

The player emits a `canplay` event when the `Player` has obtained just enough video frames and is obtaining them quickly enough for smooth playback. The event handler is then passed an `Event` object. The Player reference is accessible from the event’s target member.

```
player. addEventListener('canplay', (ev) => {
    // Handle event.
})
```

#### ended

The player emits an `ended` event when playback of the Live Photo has completed. The event handler is then passed an `Event` object. The Player reference is accessible from the event’s target member.

```
player.addEventListener('ended', (ev) => {
    // Handle event.
})
```

#### error

The player emits an `error` event when loading of either the photo or video components of the Live Photo has failed. The event handler is then passed an `Event` object, which has a detail member containing error information. If LivePhotosKit JS cannot interpret an internal exception, the `error` member of `detail` will be the exception object. The `Player` reference may be obtained from the event’s target member.

```
player.addEventListener('error', (ev) => {
    if (typeof ev.detail.errorCode === 'number') {
        switch (ev.detail.errorCode) {
        case LivePhotosKit.Errors.IMAGE_FAILED_TO_LOAD:
            // Do something
            break;
        case LivePhotosKit.Errors.VIDEO_FAILED_TO_LOAD:
            // Do something
            break;
        }
    } else {
        // Extract Error object.
        console.error(ev.detail.error);
    }
})
```

## Topics

### Initializers

LivePhotosKit.Player

Creates `LivePhotosKit.Player` objects.

### Instance Properties

currentTime

The current time, in seconds, of the play head.

duration

The duration, in seconds, of the entire Live Photo.

photoHeight

The height, in pixels, of the photo component.

photoTime

The nominated time, in seconds, of where the photo component should be within the Live Photo video component.

photoWidth

The width, in pixels, of the photo component.

canPlay

A Boolean value that indicates whether the Player is able to begin playback.

errors

An array of errors that occurred when attempting to load resources.

frameTimes

An array of timestamps for each second from the beginning of a Live Photo for which the frames reside in the Live Photo.

isPlaying

A Boolean value that indicates whether or not the Player is playing.

loadProgress

A numeric value that indicates the progress of loading the Live Photo.

metadataVideoSrc

A string or array buffer that contains metadata about the properties of a Live Photo.

photo

The renderable, image-bearing DOM element (either an image or a canvas) that the Player consumes to render itself to the screen.

photoMimeType

The MIME type of a photo asset.

photoSrc

The source of the photo component of the Live Photo.

playbackStyle

The style of playback that determines the nature of an animation.

proactivelyLoadsVideo

A boolean value that indicates whether the Player downloads bytes before the user begins playback.

renderedTime

The current timestamp, as a floating-point number of seconds from the beginning of the animation, that is truly displayed on the screen.

showsNativeControls

The value of this property indicates whether the Apple-provided playback controls are enabled for the user.

video

The playable `HTMLVideoElement` that the Player consumes to obtain video frame data to render to the screen while animating a Live Photo.

videoHeight

The height, in pixels, of the underlying video asset provided to the Player.

videoMimeType

The MIME type of the video asset.

videoRotation

The angle that the video is displayed.

videoSrc

A reference to the source of the video component of this Live Photo.

videoWidth

The width, in pixels, of an underlying video asset provided to the Player.

wantsToPlay

A boolean that indicates whether the Player has been instructed to play.

autoplay

effectType

### Instance Methods

beginFinishingPlaybackEarly

Clips the duration of the renderer early so that the animation begins to fade back to the photo component earlier than it would ordinarily.

pause

Pauses playback at the current time.

play

Starts playback if the player is ready, or resumes playback if the player is paused.

stop

Stops playback and rewinds to the current time of zero.

toggle

Starts playing the video component of Live Photo if the video is paused, or pauses the video if it is playing.

updateSize

Updates the size of the player.

## See Also

### Classes

LivePhotosKit

The namespace for the LivePhotosKit library.

