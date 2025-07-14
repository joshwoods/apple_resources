

- TVMLKit
-  TVPlaybackEventMarshaling Deprecated

Protocol

# TVPlaybackEventMarshaling

A protocol used for sending and receiving information across the JavaScript bridge.

tvOS 12.0–18.0Deprecated

``` source
protocol TVPlaybackEventMarshaling : NSObjectProtocol
```

Deprecated

Please use SwiftUI or UIKit

## Overview

You must conform to this protocol in order to pass custom events.

## Topics

### Processing Playback Events

func processReturnValue(value: JSValue, in: JSContext)

Converts a JavaScript value into a value that is readable in Swift or Objective-C.

var properties: [TVPlaybackEventProperty : Any]?

An array of custom playback event properties.

**Required**

struct TVPlaybackEventProperty

Extend this structure to create your own custom playback event properties.

## Relationships

### Inherits From

- NSObjectProtocol

### Conforming Types

- TVPlaybackCustomEventUserInfo

## See Also

### Controlling Playback

func next()

Plays the next media item in the playlist.

Deprecated

func pause()

Pauses the currently playing item.

Deprecated

func previous()

Plays the previous media item in the playlist.

Deprecated

var state: TVPlaybackState

The current state of the player.

Deprecated

enum TVPlaybackState

The possible states of a player.

Deprecated

func dispatch(event: TVPlaybackEvent, userInfo: (any TVPlaybackEventMarshaling)?, completion: ((Bool) -> Void)?)

Dispatches custom playback events to the JavaScript environment.

Deprecated

struct TVPlaybackEvent

Extend this structure to send your custom playback events to the JavaScript environment.

Deprecated

class TVPlaybackCustomEventUserInfo

The user information used in a custom playback event.

Deprecated

