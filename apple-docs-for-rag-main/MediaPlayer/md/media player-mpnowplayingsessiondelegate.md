

- Media Player
-  MPNowPlayingSessionDelegate 

Protocol

# MPNowPlayingSessionDelegate

A protocol that defines the delegate interface for a Now Playing session.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+tvOS 14.0+visionOS 1.0+

``` source
protocol MPNowPlayingSessionDelegate : NSObjectProtocol
```

## Topics

### Responding to state changes

func nowPlayingSessionDidChangeActive(MPNowPlayingSession)

Tells the delegate that the session changed its active status.

func nowPlayingSessionDidChangeCanBecomeActive(MPNowPlayingSession)

Tells the delegate that the session is eligible to become active.

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### Accessing the delegate object

var delegate: (any MPNowPlayingSessionDelegate)?

The Now Playing session’s delegate object.

