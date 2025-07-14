

- TVMLKit JS
-  Player 

Class

# Player

A media player that displays the UI for playing video and audio in an Apple TV client-server app.

tvOS 9.0+

``` source
interface Player
```

## Overview

After you create a new player, associate the player with a playlist that contains media items. In order to play audio or video, at a minimum, there must be a `Player` object that contains a single Playlist object, which contains a single MediaItem object.

## Topics

### Setting Up the Player

interactiveOverlayDismissable

Determines if an interactive overlay can be dismissed using the Menu button.

interactiveOverlayDocument

A DOM document that is presented over the entire video player, including the transport bar.

overlayDocument

The annotations for a video created by placing a DOM document over the video.

Player

Creates a new player object.

playlist

The playlist for a player.

present

Shows the player UI if it is not currently visible.

### Controlling Playback

changeToMediaAtIndex

Immediately begins playing the media item at the specified index in the playlist.

pause

Pauses the currently playing media item.

next

Immediately begins playing the next media item in the playlist.

play

Plays the currently selected media item.

playbackState

The current state of the player.

playbackRate

The playback speed.

previous

Immediately begins playing the previous media item in the playlist.

seekToTime

Sets the playback point to a specified time.

stop

Stops the currently playing item and dismisses the player UI.

### Inspecting Media Items

currentMediaItem

The currently selected media item in the playlist.

currentMediaItemDate

Contains the current time of the media item as a `Date` object.

currentMediaItemDuration

The length, in seconds, of the current media item.

nextMediaItem

The next media item in the playlist after the currently selected item.

previousMediaItem

The item in the playlist previous to the currently selected item.

### Responding to Events

mediaItemDidChange

An event notifying the listener that the player changed a media item.

mediaItemWillChange

An event notifying the listener that the player is about to changed a media item.

playbackDidStall

An event that indicates that playback has stalled.

playbackError

An event that indicates an error has occurred during playback.

requestSeekToTime

An event that indicates whether a seek-to-time request was accomplished.

shouldChangeToMediaAtIndex

An event that indicates a request to play a media item in a different index is received.

shouldHandleStateChange

An event that indicates a state change request has occurred.

stateDidChange

An event that indicates the state of the player has changed.

stateWillChange

An event that indicates the state of the player is about to change.

timeBoundaryDidCross

An event that indicates a specific playback time in the media item has been crossed.

timeDidChange

An event that happens at a specified interval.

timedMetadata

An event that is triggered whenever a specified piece of metadata is encountered.

transportBarVisibilityDidChange

An event that indicates the state of the transport bar has changed.

## Relationships

### Inherits From

- EventListenerObject

## See Also

### Media Playback

Playing Media in a Client-Server App

Play media items in a client-server app using the built-in media player for TVMLKit JS.

Playlist

An array of media items to be played in an Apple TV client-server app.

MediaItem

A single audio or video item.

Slideshow

An object used to display images on Apple TV in a slideshow format.

Browser

An object used to configure and present a browsable full screen view.

