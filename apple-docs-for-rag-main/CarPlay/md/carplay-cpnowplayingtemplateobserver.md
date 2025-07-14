

- CarPlay
-  CPNowPlayingTemplateObserver 

Protocol

# CPNowPlayingTemplateObserver

The methods for responding to the user interacting with the Now Playing template.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+

``` source
protocol CPNowPlayingTemplateObserver : NSObjectProtocol
```

## Overview

You use a Now Playing template observer to respond when the user interacts with the Album-Artist and Up Next buttons. The protocol defines methods that CarPlay calls when a user taps these buttons. Use your implementation to provide the appropriate behavior when these events occur. For example, when the user taps the Album-Artist button, you can present a new template that displays the content of the current album, playlist, or podcast.

To register an observer, create an object that implements the `CPNowPlayingTemplateObserver` protocol and then call the Now Playing template’s add(_:) method, passing your object as the only parameter.

## Topics

### Responding to User Interactions

func nowPlayingTemplateAlbumArtistButtonTapped(CPNowPlayingTemplate)

Tells the observer that the user tapped the Album-Artist button.

func nowPlayingTemplateUpNextButtonTapped(CPNowPlayingTemplate)

Tells the observer that the user tapped the Up Next button.

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### Observing Now Playing Events

func add(any CPNowPlayingTemplateObserver)

Registers an observer that receives Now Playing template events.

func remove(any CPNowPlayingTemplateObserver)

Removes an observer from receiving Now Playing template events.

