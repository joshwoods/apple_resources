

- Media Player
- MPNowPlayingSession
-  becomeActiveIfPossible(completion:) 

Instance Method

# becomeActiveIfPossible(completion:)

Tells the system to make the session the active Now Playing session if possible.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+tvOS 14.0+visionOS 1.0+

``` source
func becomeActiveIfPossible(completion: ((Bool) -> Void)? = nil)
```

``` source
func becomeActiveIfPossible() async -> Bool
```

## Parameters 

`completion`  

The completion handler the system calls after it processes the request.

## See Also

### Managing the active state

var isActive: Bool

A Boolean value that indicates whether the session is the app’s active Now Playing session.

var canBecomeActive: Bool

A Boolean value that indicates whether the session can become the app’s active Now Playing session.

