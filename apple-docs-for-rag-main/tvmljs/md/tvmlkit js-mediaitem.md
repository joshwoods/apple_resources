

- TVMLKit JS
-  MediaItem 

Class

# MediaItem

A single audio or video item.

tvOS 9.0+

``` source
interface MediaItem
```

## Overview

In order to play audio or video, at a minimum, there must be a Player object that contains a single Playlist object which contains a single `MediaItem` object.

## Topics

### Creating Media Items

MediaItem

Creates a new `MediaItem` object from the information stored in the URL location.

### Rating Media Content

contentRatingDomain

The domain that the rating applies to.

contentRatingRanking

The rating for a video item.

isExplicit

A Boolean value indicating whether the item has explicit lyrics.

### Identifying Media Items

artworkImageURL

The URL path to the artwork that accompanies the media item.

description

The description for a media item.

subtitle

The subtitle for a the media item.

title

The title of the media item.

type

The type of media item.

url

The URL path to the media item.

### Setting Timing Options

highlightGroups

An array of highlight groups, with each group containing a list of highlights.

interstitials

An array of `interstitial` objects.

resumeTime

The number of seconds from the beginning of the item at which the item begins playing.

### Supporting FairPlay Streaming

loadAssetID

A callback function used to load the asset identifier for an item.

loadCertificate

A callback function used to load the security certificate for an item.

loadKey

A callback function used to load the security key for an item.

## See Also

### Media Playback

Playing Media in a Client-Server App

Play media items in a client-server app using the built-in media player for TVMLKit JS.

Player

A media player that displays the UI for playing video and audio in an Apple TV client-server app.

Playlist

An array of media items to be played in an Apple TV client-server app.

Slideshow

An object used to display images on Apple TV in a slideshow format.

Browser

An object used to configure and present a browsable full screen view.

