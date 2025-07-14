

- Media Player
-  MPNowPlayingSession 

Class

# MPNowPlayingSession

An object that manages Now Playing information and remote commands for multiple players.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+tvOS 14.0+visionOS 1.0+

``` source
class MPNowPlayingSession
```

## Overview

An AVPlayer object can have only one Now Playing session. An AVPlayerViewController manages its own player and Now Playing session, so you can’t add your own Now Playing session.

Important

If you create an `MPNowPlayingSession` object, don’t attempt to use it with the `AVPlayer` that an `AVPlayerViewController` presents. Create your own `AVPlayer` instance with custom playback controls to use with your Now Playing session.

## Topics

### Creating a session

init(players: [AVPlayer])

Creates a Now Playing session object.

### Accessing the delegate object

var delegate: (any MPNowPlayingSessionDelegate)?

The Now Playing session’s delegate object.

protocol MPNowPlayingSessionDelegate

A protocol that defines the delegate interface for a Now Playing session.

### Managing players

var players: [AVPlayer]

The array of players associated with the session.

func addPlayer(AVPlayer)

Adds a player to the session.

func removePlayer(AVPlayer)

Removes a player from the session.

### Managing the active state

var isActive: Bool

A Boolean value that indicates whether the session is the app’s active Now Playing session.

var canBecomeActive: Bool

A Boolean value that indicates whether the session can become the app’s active Now Playing session.

func becomeActiveIfPossible(completion: ((Bool) -> Void)?)

Tells the system to make the session the active Now Playing session if possible.

### Configuring Now Playing information

var automaticallyPublishesNowPlayingInfo: Bool

A Boolean that indicates whether Now Playing info automatically publishes.

var nowPlayingInfoCenter: MPNowPlayingInfoCenter

The Now Playing information center associated with the session.

### Handling remote commands

var remoteCommandCenter: MPRemoteCommandCenter

The remote command center associated with the session.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Now Playing information

Becoming a now playable app

Ensure your app is eligible to become the Now Playing app by adopting best practices for providing Now Playing info and registering for remote command center actions.

class MPNowPlayingInfoCenter

An object for setting the Now Playing information for media that your app plays.

class MPNowPlayingInfoLanguageOption

A set of interfaces for setting the language option for the Now Playing item.

class MPNowPlayingInfoLanguageOptionGroup

A grouped set of language options where only a single language option can be active at a time.

Language option characteristic constants

The constants for defining language characteristics.

