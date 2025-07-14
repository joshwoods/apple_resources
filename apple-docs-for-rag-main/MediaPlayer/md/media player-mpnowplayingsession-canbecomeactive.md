

- Media Player
- MPNowPlayingSession
-  canBecomeActive 

Instance Property

# canBecomeActive

A Boolean value that indicates whether the session can become the app’s active Now Playing session.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+tvOS 14.0+visionOS 1.0+

``` source
var canBecomeActive: Bool { get }
```

## See Also

### Managing the active state

var isActive: Bool

A Boolean value that indicates whether the session is the app’s active Now Playing session.

func becomeActiveIfPossible(completion: ((Bool) -> Void)?)

Tells the system to make the session the active Now Playing session if possible.

