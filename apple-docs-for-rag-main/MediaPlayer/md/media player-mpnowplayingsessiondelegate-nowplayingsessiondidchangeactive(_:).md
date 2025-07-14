

- Media Player
- MPNowPlayingSessionDelegate
-  nowPlayingSessionDidChangeActive(\_:) 

Instance Method

# nowPlayingSessionDidChangeActive(\_:)

Tells the delegate that the session changed its active status.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+tvOS 14.0+visionOS 1.0+

``` source
optional func nowPlayingSessionDidChangeActive(_ nowPlayingSession: MPNowPlayingSession)
```

## Parameters 

`nowPlayingSession`  

The Now Playing session that changed.

## See Also

### Related Documentation

var isActive: Bool

A Boolean value that indicates whether the session is the app’s active Now Playing session.

### Responding to state changes

func nowPlayingSessionDidChangeCanBecomeActive(MPNowPlayingSession)

Tells the delegate that the session is eligible to become active.

