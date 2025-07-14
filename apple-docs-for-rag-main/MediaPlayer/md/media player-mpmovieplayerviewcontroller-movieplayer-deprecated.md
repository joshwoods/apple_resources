

- Media Player
- MPMoviePlayerViewController
-  moviePlayer Deprecated

Instance Property

# moviePlayer

The movie player controller object used to present the movie.

iOS 3.2–9.0DeprecatediPadOS 3.2–9.0DeprecatedMac Catalyst 13.1–13.1Deprecated

``` source
@MainActor
var moviePlayer: MPMoviePlayerController! { get }
```

Deprecated

Use AVPlayerViewController in AVKit.

## Discussion

The MPMoviePlayerController object in this property is created automatically by the receiver and cannot be changed. However, you can use the object to manage the presentation and configuration of the movie playback.

## See Also

### New methods

init!(contentURL: URL!)

Returns a movie player view controller initialized with the specified movie.

Deprecated

