

- TVMLKit JS
-  Playlist 

Class

# Playlist

An array of media items to be played in an Apple TV client-server app.

tvOS 9.0+

``` source
interface Playlist
```

## Overview

In order to play audio or video, at a minimum, there must be a Player object that contains a single `Playlist` object, which contains a single MediaItem object.

## Topics

### Modifying the Playlist

item

Returns the media item located in the indicated array index.

length

The number of items in the playlist.

Playlist

Creates a new playlist object.

pop

Removes a media item from the end of a playlist.

push

Adds a media item to the end of a playlist.

splice

Deletes the indicated array elements and replaces them with the specified elements.

## See Also

### Media Playback

Playing Media in a Client-Server App

Play media items in a client-server app using the built-in media player for TVMLKit JS.

Player

A media player that displays the UI for playing video and audio in an Apple TV client-server app.

MediaItem

A single audio or video item.

Slideshow

An object used to display images on Apple TV in a slideshow format.

Browser

An object used to configure and present a browsable full screen view.

