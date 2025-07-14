

- Media Player
- MPMoviePlayerViewController
-  init(contentURL:) Deprecated

Initializer

# init(contentURL:)

Returns a movie player view controller initialized with the specified movie.

iOS 3.2–9.0DeprecatediPadOS 3.2–9.0DeprecatedMac Catalyst 13.1–13.1Deprecated

``` source
@MainActor
init!(contentURL: URL!)
```

Deprecated

Use AVPlayerViewController in AVKit.

## Parameters 

`contentURL`  

The URL that points to the content to be played.

## Return Value

A movie player view controller initialized with the specified URL.

## See Also

### New methods

var moviePlayer: MPMoviePlayerController!

The movie player controller object used to present the movie.

Deprecated

