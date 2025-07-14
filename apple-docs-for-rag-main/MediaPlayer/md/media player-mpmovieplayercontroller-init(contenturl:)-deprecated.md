

- Media Player
- MPMoviePlayerController
-  init(contentURL:) Deprecated

Initializer

# init(contentURL:)

Returns a `MPMoviePlayerController` object initialized with the movie at the specified URL.

iOS 3.2–9.0DeprecatediPadOS 3.2–9.0DeprecatedMac Catalyst 13.1–13.1Deprecated

``` source
init!(contentURL url: URL!)
```

Deprecated

Use AVPlayerViewController in AVKit

## Parameters 

`url`  

The location of the movie file. This file must be located either in your app directory or on a remote server.

## Return Value

The movie player object.

## Discussion

This method initializes a movie player, but does not prepare it for playback. To prepare a new movie player for playback, call the prepareToPlay() method, described in MPMediaPlayback.

To be notified when a new movie player is ready to play, register for the MPMoviePlayerLoadStateDidChangeNotification notification. You can then check load state by accessing the loadState property.

To check for errors in URL loading, register for the MPMoviePlayerPlaybackDidFinishNotification notification. On error, this notification contains an NSError object available using the `@"error"` key in the notification’s `userInfo` dictionary.

