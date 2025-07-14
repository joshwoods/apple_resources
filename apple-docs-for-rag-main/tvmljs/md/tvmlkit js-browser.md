

- TVMLKit JS
-  Browser 

Class

# Browser

An object used to configure and present a browsable full screen view.

tvOS 13.0+

``` source
interface Browser
```

## Overview

There is no constructor for this object. Configure the `Browser` by modifying its properties. When appropriately configured, use the `present `method to display a new `Browser`.

## Topics

### Creating a Browser

present

Shows the Browser UI if it is not currently visible.

### Modifying a Browser

maskInset

The insets from the edges of the full screen layout.

interitemSpacing

The spacing between full screen browser items.

cornerRadius

The corner radius of each full screen browser item.

## See Also

### Media Playback

Playing Media in a Client-Server App

Play media items in a client-server app using the built-in media player for TVMLKit JS.

Player

A media player that displays the UI for playing video and audio in an Apple TV client-server app.

Playlist

An array of media items to be played in an Apple TV client-server app.

MediaItem

A single audio or video item.

Slideshow

An object used to display images on Apple TV in a slideshow format.

